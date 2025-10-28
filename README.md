# Claude Code Template for Awesome Lists

A template repository designed to streamline the creation of high-quality curated resource lists ("Awesome Lists") using Claude Code.

## Purpose

This template isn't about generating spammy lists for the sake of it. Instead, it provides a structured workflow to help you:

- **Create meaningful resource collections** - Whether for your own reference or community sharing
- **Maintain consistent quality** - Through automated formatting and organization
- **Save time on structure** - Focus on curation, not formatting
- **Keep lists up-to-date** - With tools to help refresh content systematically

**Use cases:**
- Personal reference collections (private repos)
- Open source community resources (public repos)
- Team knowledge bases
- Research resource compilations

## What's Included

### Slash Commands

This template includes custom Claude Code slash commands in `.claude/commands/`:

- **`scratchpad-to-list.md`** - Transforms unstructured notes from a scratchpad into a well-organized README with:
  - Logical section organization
  - Alphabetical ordering within sections
  - Shields.io badges (View Repo, Star Count, Last Commit)
  - Table of contents for larger lists
  - Automated description fetching from repositories
  - Consistent formatting with horizontal rule dividers

**Note:** The `.gitignore` is configured to exclude personal Claude Code settings (like `.claude/settings.local.json`) while including the shared commands directory. This balances security with sharing.

## Getting Started

1. **Clone or fork this repository**
   ```bash
   git clone <your-fork-url>
   cd Claude-Is-Awesome
   ```

2. **The slash commands are ready to use** - No installation needed! Just open Claude Code in this directory.

## Usage

### Creating Your Awesome List

1. **Use the scratchpad** (`scratchpad.txt` or create your own)
   - Add repository URLs or names
   - Note section categories
   - Include your observations and descriptions
   - Don't worry about formatting

2. **Run the slash command**
   ```
   /scratchpad-to-list
   ```

3. **Review and refine**
   - Claude Code will organize everything into a structured README
   - Verify the categories and ordering make sense
   - Add any final touches

### Working with Data

The `data/` directory is included for:
- Storing research notes
- Keeping CSV/JSON exports
- Managing metadata about your list
- Version controlling supplementary information

## Why This Approach Works

**Quality over quantity**: By automating the tedious parts (formatting, badge generation, alphabetizing), you can focus on the curation itself - finding valuable resources and explaining why they matter.

**Flexibility**: Whether you're building a public awesome list for the community or a private collection for your own use, the workflow adapts to your needs.

**Maintainability**: Structured data in the scratchpad makes it easy to update and expand your list over time.

## Best Practices

- **Be selective**: Only include resources you've reviewed or have reason to believe are valuable
- **Add context**: Your observations and descriptions help others understand why resources matter
- **Regular updates**: Revisit your scratchpad periodically to add new discoveries
- **Clear categorization**: Think about how users will want to browse your list

## Repository Structure

```
.
├── .claude/
│   └── commands/          # Claude Code slash commands (shared)
├── data/                  # Supporting data and notes
├── backups/              # Backup storage (gitignored)
├── scratchpad.txt        # Your working notes
├── .gitignore            # Excludes .claude/* except commands/
└── README.md             # This file (or your awesome list)
```

## Contributing to This Template

If you've created additional slash commands or workflows that improve the awesome list creation process, contributions are welcome. Open an issue or pull request with your suggestions.

To add your own slash commands, just create `.md` files in `.claude/commands/` - they'll automatically be available when you run Claude Code.

## License

MIT License - Feel free to use this template for any purpose, public or private.

## Credits

Built to work with [Claude Code](https://claude.ai/code) by Anthropic.
