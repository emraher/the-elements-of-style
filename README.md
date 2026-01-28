# The Elements of Style - Claude Code Plugin

A Claude Code plugin that distills William Strunk Jr.'s *The Elements of Style* (1918) into a practical writing reference for technical documentation, user-facing text, and any prose.

## What This Plugin Does

Gives Claude access to Strunk's writing principles in a token-efficient format. When Claude writes documentation, commit messages, error messages, or other prose, it consults these rules.

## Installation

```bash
# Clone into your Claude Code plugins directory
cd ~/.claude/plugins  # or your plugins directory
git clone https://github.com/emraher/the-elements-of-style.git
```

Claude automatically detects and uses the skill when appropriate.

This is an enhanced fork of [obra/elements-of-style](https://github.com/obra/elements-of-style) with 87% token reduction, expanded technical examples, and 100+ example demonstrations.

## The Rules

Elementary Rules of Usage (Grammar/Punctuation):
1. Form possessive singular by adding 's
2. Use comma after each term in series except last
3. Enclose parenthetic expressions between commas
4. Comma before conjunction introducing co-ordinate clause
5. Don't join independent clauses by comma
6. Don't break sentences in two
7. Participial phrase at beginning refers to grammatical subject

Elementary Principles of Composition:
8. One paragraph per topic
9. Begin paragraph with topic sentence
10. Use active voice
11. Put statements in positive form
12. Use definite, specific, concrete language
13. Omit needless words
14. Avoid succession of loose sentences
15. Express co-ordinate ideas in similar form
16. Keep related words together
17. Keep to one tense in summaries
18. Place emphatic words at end

Rules 10-13 and 16 matter most for technical writing.

## Before & After Example

Before (Passive, vague, wordy):
> The new feature that was added to the system is not yet available to all users due to the fact that there are still some issues that need to be resolved.

After (Active, concrete, concise):
> We added a new feature but haven't released it to all users yet. Three bugs block the rollout.

Rules applied: Active voice (10), Positive form (11), Concrete language (12), Omit needless words (13)

## When Claude Uses This

Claude invokes `writing-clearly-and-concisely` when:
- Writing or editing documentation (READMEs, guides, API docs)
- Crafting commit messages or PR descriptions
- Creating error messages, logs, or UI copy
- Writing code comments or docstrings
- Explaining technical concepts
- Any task requiring prose for human readers

## What's Included

- All 18 core rules with practical examples
- Before/after comparisons for every major rule
- Technical writing examples: Git commits, API docs, error messages, code comments
- Common mistakes: Word usage (data/datum, less/fewer, like/as, effect/affect)
- 100+ example demonstrations of good and bad writing
- 300-token quick reference for fast lookup

## Token Efficiency

The original 1918 text is ~50,000 words. This plugin condenses it to:
- quick-reference.md: ~300 tokens (fast lookup)
- SKILL.md: ~600 tokens (when to use guide)
- elements-of-style.md: ~1,400 tokens (complete guide with examples)

Comparison:
- Original full text: ~25,000 tokens
- This plugin: 300-1,400 tokens (94-98% reduction)

This makes the guidance cheap enough to consult frequently rather than only when context allows.

## Source & License

Based on William Strunk Jr.'s 1918 edition, obtained from [Project Gutenberg #37134](https://www.gutenberg.org/files/37134/37134-h/37134-h.htm).

License: Public Domain (see LICENSE file)

Original Text: William Strunk Jr. (1918)

Initial Plugin: Jesse Vincent ([obra/elements-of-style](https://github.com/obra/elements-of-style))

Enhanced & Maintained: emraher ([emraher/the-elements-of-style](https://github.com/emraher/the-elements-of-style))

Enhancements in v2.0.0: 87% token reduction, technical writing examples, quick reference, example suite. See CHANGELOG.md for details.

## Contributing

Issues and pull requests welcome at [github.com/emraher/the-elements-of-style](https://github.com/emraher/the-elements-of-style).

When contributing:
- Maintain token efficiency (measure before/after)
- Add technical writing examples where relevant
- Follow Strunk's rules in your own writing
- Include examples for new content
