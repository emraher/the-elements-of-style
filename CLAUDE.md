# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## What This Repository Is

This is a Claude Code plugin that packages William Strunk Jr.'s *The Elements of Style* (1918) as a reusable skill. The plugin gives Claude Code instances access to Strunk's writing guidance for documentation, user-facing text, or any prose.

**Repository**: https://github.com/emraher/the-elements-of-style (v2.0.0)
**Original**: https://github.com/obra/elements-of-style (v1.0.0 by Jesse Vincent)

This enhanced fork improves the original with 87% token reduction, technical writing examples, quick reference card, and comprehensive example suite.

## Architecture

The repository follows the Claude Code plugin structure:

```
.claude-plugin/
  plugin.json          # Plugin metadata (name, version, description, author)

skills/
  writing-clearly-and-concisely/
    SKILL.md           # Skill invocation guide (~600 tokens)
    elements-of-style.md  # Full reference text (~12,000 tokens)
```

### Key Design Decisions

**Three-tier approach**: The skill is split across three reference files for different contexts:
1. **quick-reference.md** (~300 tokens): Ultra-condensed for fast lookup when context is extremely tight
2. **SKILL.md** (~600 tokens): When to use the skill and all 18 rules at a glance
3. **elements-of-style.md** (~1,400 tokens): Complete guide with all rules, examples, and technical writing guidance

The reference was heavily condensed from the original ~25,000 tokens (94% reduction) by:
- Removing verbose explanations and lengthy literary examples
- Keeping only essential grammar/punctuation rules with brief examples
- Focusing on the most impactful composition rules (10-13, 16, 18)
- Condensing "Words Commonly Misused" into grouped categories
- Adding specific technical writing examples (commits, API docs, error messages)
- Creating a comprehensive example suite separate from the reference material

**Public domain content**: The 1918 edition predates modern style guides. The original was sourced from Project Gutenberg #37134 and heavily condensed for token efficiency.

**Repository history**: Originally created by Jesse Vincent (obra/elements-of-style), now enhanced and maintained by emraher (emraher/the-elements-of-style) with major improvements in v2.0.0.

## Files and Their Purpose

- `skills/writing-clearly-and-concisely/quick-reference.md`: Ultra-condensed reference (~300 tokens) for fast lookup
- `skills/writing-clearly-and-concisely/SKILL.md`: Invocation guide (~600 tokens) listing when to use the skill
- `skills/writing-clearly-and-concisely/elements-of-style.md`: Complete condensed guide (~1,400 tokens) with all 18 rules, examples, and technical writing guidance
- `examples/writing-examples.md`: Test suite with 100+ good/bad examples demonstrating each rule
- `.claude-plugin/plugin.json`: Plugin metadata (version 2.0.0)

## No Build Process

This is a pure content repository. There are no dependencies, build steps, or tests. The plugin works through Claude Code's plugin system by placing it in the plugins directory.

## Editing the Content

If you need to modify the writing guidance:

1. **For structural changes** (when to use the skill, invocation strategy): Edit `SKILL.md`
2. **For content changes** (Strunk's actual rules and examples): Edit `elements-of-style.md`
3. **For metadata** (plugin name, version, description): Edit `.claude-plugin/plugin.json`

When editing `elements-of-style.md`, maintain the token-efficient format. The original source is available at Project Gutenberg #37134 if you need to reference the full text.

## The Source Material

Strunk's guide has three sections:

1. **Elementary Rules of Usage** (Rules 1-7): Grammar and punctuation fundamentals
2. **Elementary Principles of Composition** (Rules 8-18): Writing clarity and structure
3. **Words and Expressions Commonly Misused**: Alphabetical usage reference

The most impactful rules for technical writing:
- Rule 10: Use active voice
- Rule 11: Put statements in positive form
- Rule 12: Use definite, specific, concrete language
- Rule 13: Omit needless words

These are bolded in SKILL.md because they apply to nearly all technical prose.
