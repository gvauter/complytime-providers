---
pack_id: default-custom
language: Any
version: 1.0.0
---
<!-- scaffolded by uf vv0.12.0 -->

# Custom Rules: Default

Project-specific conventions that extend the canonical
default convention pack. Rules in this file are loaded alongside
`default.md` by Cobalt-Crush (during implementation) and
all Divisor persona agents (during review).

Use the `CR-NNN` prefix for all custom rules. Use `[MUST]`,
`[SHOULD]`, or `[MAY]` severity indicators per RFC 2119.

## Custom Rules

<!-- Add project-specific rules below this line -->

### CR-001: Git Commit Signing [MUST]

All git commits MUST use both `-S` (GPG/SSH sign) and `-s` (Signed-off-by) flags.
The correct invocation is always `git commit -S -s -m "message"`.
Never create a commit without both flags.

### CR-002: AI Assisted-by Trailer [MUST]

All git commits MUST include an `Assisted-by: OpenCode (claude-opus-4-6)` trailer
in the commit message.
