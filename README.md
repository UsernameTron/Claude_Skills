# Claude Skills Development Project

## Overview
This project contains custom Claude skills for enhancing Claude's capabilities in document processing, project management, and workflow automation.

## Skills Included

### 1. **asana-support**
End-to-end Asana assistance for users, managers, and admins covering setup, workflow design, reporting, governance, and AI usage.

### 2. **docx-advanced**
Advanced Microsoft Word document manipulation and processing capabilities.

### 3. **pdf-advanced**
Enhanced PDF processing, manipulation, and analysis tools.

### 4. **pptx-advanced**
Advanced PowerPoint presentation creation and modification capabilities.

### 5. **xlsx-advanced**
Sophisticated Excel spreadsheet processing and data analysis features.

## Project Structure

```
Claude Skills/
├── README.md                 # This file
├── PROJECT_SETUP.md         # Development setup guide
├── extracted/               # Extracted skill contents
│   ├── asana-support/
│   ├── docx-advanced/
│   ├── pdf-advanced/
│   ├── pptx-advanced/
│   └── xlsx-advanced/
├── scripts/                 # Utility scripts
│   ├── extract_all.sh      # Extract all zip files
│   ├── validate_skills.py  # Validate skill structure
│   └── package_skills.sh   # Repackage skills
└── *.zip                   # Original skill packages
```

## Claude Code Integration

This project is optimized for Claude Code coding assistant. Key features:

- **Modular Structure**: Each skill is self-contained with its SKILL.md
- **Clear Documentation**: Every skill includes comprehensive usage docs
- **Version Control Ready**: Extracted skills are ready for git tracking
- **Development Scripts**: Automated tools for skill management

## Quick Start for Claude Code

### Extract All Skills
```bash
cd /Users/cpconnor/projects/Claude\ Skills
./scripts/extract_all.sh
```

### Validate Skill Structure
```bash
python3 scripts/validate_skills.py
```

### View a Specific Skill
```bash
cd extracted/asana-support
cat SKILL.md
```

## Development Workflow

1. **Modify Skills**: Edit SKILL.md files in the `extracted/` directory
2. **Test Changes**: Use Claude Code to test skill modifications
3. **Validate**: Run validation scripts to ensure structure integrity
4. **Package**: Use package script to create new .zip files
5. **Deploy**: Upload packaged skills to Claude

## Skill Structure

Each skill follows this structure:

```markdown
---
name: skill-name
description: "Brief skill description"
license: Proprietary. See LICENSE.txt
---

# Skill Name

## Purpose
Clear explanation of what the skill does

## Key Features
- Feature 1
- Feature 2

## Usage Examples
...
```

## Best Practices

- Keep SKILL.md files focused and concise
- Use clear section headers for navigation
- Include decision trees for complex workflows
- Provide code examples where applicable
- Document any external dependencies
- Version control all changes

## Contributing

When modifying skills:
1. Update the SKILL.md with clear documentation
2. Test with Claude Code to ensure functionality
3. Update this README if adding new skills
4. Maintain backward compatibility when possible

## License

See individual skill LICENSE.txt files for licensing information.

---
*Optimized for Claude Code development*
