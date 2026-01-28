# Changelog

All notable changes to this project will be documented in this file.

## [2.0.0] - 2025-01-28

### Changes
- **87% token reduction**: Main guide reduced from ~25,000 tokens to ~1,400 tokens
- **Three-tier reference system**:
  - Quick reference (300 tokens)
  - Skill guide (600 tokens)
  - Complete guide (1,500 tokens)
- **Repository transfer**: Forked from obra/elements-of-style, now maintained by emraher

### Added
- `quick-reference.md`: 300-token version for quick lookup
- `examples/writing-examples.md`: Test suite with 100+ before/after examples
- Technical writing examples for:
  - Git commit messages
  - API documentation
  - Error messages
  - Code comments
  - General documentation
- Section numbers (II, III, V) to clarify rule categories
- Stars (⭐) highlighting most impactful rules for technical writing
- Real-world impact examples in README
- Token efficiency comparison metrics
- Installation instructions with git clone
- Contributing guidelines

### Changed
- Condensed "Words Commonly Misused" section from 30 entries to grouped categories
- Enhanced README with before/after examples and real-world impact
- Updated SKILL.md to reference three-tier system
- Expanded technical writing section with 6 categories of examples
- Updated all repository URLs from obra → emraher
- Added contributors section crediting Jesse Vincent

### Removed
- `elements-of-style.html`: Original Project Gutenberg HTML (no longer needed)
- Verbose explanations and lengthy literary examples
- Outdated "dispatch subagent" strategy (no longer needed with 1,500 tokens)
- Less relevant words from misused words section

### Improved
- Plugin metadata: version 2.0.0, enhanced description, technical-writing keyword
- CLAUDE.md: Comprehensive architecture documentation
- File organization: Clear separation of references, tests, and metadata

## [1.0.0] - Original Release (Jesse Vincent)

### Added
- Initial plugin structure
- Complete 1918 text from Project Gutenberg
- Basic markdown conversion
- Plugin metadata and configuration

---

**Repository**: https://github.com/emraher/the-elements-of-style
**Original**: https://github.com/obra/elements-of-style
**Source Text**: Project Gutenberg #37134 (Public Domain)
