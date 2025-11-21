# CLAUDE.md - AI Assistant Development Guide

## Repository Overview

This repository contains the privacy policy page for **DinarChange**, a currency exchange application. The project is a simple, single-page HTML document that presents the application's privacy policy in French (RGPD/GDPR compliant).

### Project Purpose
- Display the privacy policy for the DinarChange mobile application
- Provide transparency about data collection and usage
- Comply with RGPD (General Data Protection Regulation) requirements
- Meet App Store privacy policy requirements

### Key Information
- **Application Name**: DinarChange (Currency Exchange)
- **Language**: French
- **Compliance**: RGPD/GDPR
- **Contact Email**: dinarchange@gmail.com
- **Website**: https://changedinar.online/
- **Last Updated**: 16/02/2025

## Repository Structure

```
-privacy-policy/
├── .git/                    # Git version control
├── README.md               # Basic repository description
├── index.html              # Main privacy policy page (single-page application)
└── CLAUDE.md              # This file - AI assistant guide
```

### File Details

#### index.html (7,671 bytes)
The main and only content file containing:
- Complete HTML5 structure
- Embedded CSS (no external stylesheets)
- Responsive design (mobile-friendly)
- French language privacy policy content
- 10 main sections covering all privacy aspects

## Codebase Architecture

### Technology Stack
- **Frontend**: Pure HTML5 + CSS3 (no JavaScript)
- **Styling**: Inline CSS within `<style>` tags
- **Responsive**: Media queries for mobile devices (breakpoint: 768px)
- **No Dependencies**: Zero external libraries or frameworks

### Design System

#### CSS Variables (index.html:8-13)
```css
--primary-color: #1a73e8    /* Blue accent color */
--text-color: #333          /* Dark gray text */
--bg-color: #fff            /* White background */
--secondary-bg: #f8f9fa     /* Light gray sections */
```

#### Typography
- Font Family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif
- Base Line Height: 1.6
- Heading Hierarchy: h1 (2.5rem) → h2 (varies) → h3 (varies)

#### Layout
- Max Width: 800px (centered container)
- Padding: 20px standard, 15px mobile
- Box Model: border-box universally applied

## Content Structure

### Privacy Policy Sections (index.html:128-214)

1. **Introduction** - Overview of privacy policy purpose
2. **Data Collection and Usage**
   - 2.1: Automatically collected information (technical data, network, cache)
   - 2.2: Data NOT collected (personal data, history, tracking)
3. **Data Sharing** - Confirmation of no third-party sharing
4. **Data Security** - HTTPS encryption and security measures
5. **Permissions** - Required app permissions (Internet access only)
6. **Policy Modifications** - Right to update policy
7. **Contact** - Support contact information
8. **Legal Basis** - RGPD and App Store compliance
9. **User Rights** - GDPR rights enumeration
10. **Minor Usage** - Under-13 data protection statement

## Development Workflows

### Making Changes

#### Content Updates
When updating privacy policy content:
1. **Read the entire file first** to understand current state
2. **Locate specific section** by section number (1-10)
3. **Edit using Edit tool** - preserve HTML structure
4. **Update last-updated date** in header (index.html:122)
5. **Maintain French language** - all content is in French
6. **Test responsive design** - ensure mobile compatibility

#### Style Changes
When modifying styles:
1. **Use CSS variables** where applicable (index.html:8-13)
2. **Test at 768px breakpoint** for mobile view
3. **Maintain consistent spacing** (1.6 line-height, rem units)
4. **Preserve accessibility** (color contrast, font sizes)

### Git Workflow

#### Branch Strategy
- **Development Branch**: `claude/claude-md-mi8mab6h0gp2e1tk-01DZBQz5Q9ikq7q2qcuo9TAH`
- **Main Branch**: (default branch for PRs)
- All development work happens on Claude branches

#### Commit Guidelines
When committing changes:
```bash
# Stage changes
git add index.html

# Commit with descriptive message
git commit -m "Update privacy policy: [specific change description]"

# Push to remote (with retry logic for network issues)
git push -u origin claude/claude-md-mi8mab6h0gp2e1tk-01DZBQz5Q9ikq7q2qcuo9TAH
```

#### Commit Message Conventions
- Use descriptive, action-oriented messages
- Examples:
  - `Update privacy policy last updated date to [date]`
  - `Add new section on cookie usage`
  - `Fix responsive design issue in contact section`
  - `Update contact email address`

### Testing Checklist

Before committing changes:
- [ ] HTML validates (proper structure, closed tags)
- [ ] No broken links
- [ ] CSS renders correctly
- [ ] Responsive design works on mobile (< 768px)
- [ ] French text is grammatically correct
- [ ] Last updated date is current
- [ ] Contact information is accurate

## Key Conventions for AI Assistants

### 1. Language Considerations
- **All user-facing content MUST be in French**
- Maintain formal tone (use "nous" for first-person)
- Use proper French legal terminology
- Respect RGPD terminology (not just GDPR)

### 2. Legal Compliance
- **Never remove or weaken** existing privacy protections
- When adding new data collection, **must update** sections 2, 3, 8, 9
- Maintain transparency - be explicit about what data is collected
- Keep legal basis section (section 8) up to date

### 3. File Editing Rules
- **Always read index.html first** before making edits
- **Use Edit tool** (not Write) for modifications to existing files
- **Preserve exact indentation** (4 spaces per level)
- **Never add JavaScript** unless explicitly requested and necessary
- **Maintain inline CSS** - do not externalize styles

### 4. Date Management
- Update `last-updated` date (index.html:122) whenever content changes
- Use DD/MM/YYYY format (European date format)
- Date should reflect the actual update date

### 5. Contact Information
Current contacts (verify before using):
- **Email**: dinarchange@gmail.com (index.html:182)
- **Website**: https://changedinar.online/ (index.html:183)

**Always verify these are still valid** before making changes

### 6. Styling Principles
- Use CSS variables for colors (maintain brand consistency)
- Rem units for typography (better accessibility)
- Mobile-first thinking (test at 768px breakpoint)
- Minimal, clean design (no unnecessary embellishments)

### 7. Security Considerations
- **No external resources** - keep everything self-contained
- **No tracking scripts** - aligns with privacy-first approach
- **No forms or inputs** - static page only
- **HTTPS only** - mention in security section (index.html:160)

### 8. Common Modifications

#### Update Contact Email
```html
<!-- Find line 182 -->
<li>Email : dinarchange@gmail.com</li>
<!-- Edit to new email -->
<li>Email : newemail@example.com</li>
```

#### Add New Privacy Section
1. Insert after appropriate section (before footer)
2. Use `<section>` wrapper
3. Include `<h2>` with section number
4. Maintain consistent spacing and style
5. Update table of contents if created

#### Change Brand Colors
```css
/* Edit CSS variables at index.html:8-13 */
--primary-color: #NEW_COLOR;  /* Update this */
```

### 9. Repository Maintenance

#### When Asked to Analyze
1. Read index.html to understand current state
2. Check last-updated date for freshness
3. Verify contact information is still valid
4. Look for any broken links or references

#### When Asked to Update
1. Clarify exactly what needs updating
2. Read current content first
3. Make targeted edits (use Edit tool)
4. Update last-updated date
5. Commit with descriptive message

### 10. Things to NEVER Do
- ❌ Don't add JavaScript tracking/analytics
- ❌ Don't externalize CSS to separate file
- ❌ Don't change language from French
- ❌ Don't remove existing privacy protections
- ❌ Don't add external dependencies or CDN links
- ❌ Don't modify without reading file first
- ❌ Don't forget to update last-updated date
- ❌ Don't commit without descriptive message

## Quick Reference Commands

### File Operations
```bash
# Read the privacy policy
Read: /home/user/-privacy-policy/index.html

# Edit specific section (example: contact email)
Edit: old_string → new_string

# Check repository status
git status

# View recent changes
git log --oneline -5
```

### Development Flow
```bash
# 1. Read current state
cat index.html | grep "last-updated"

# 2. Make changes (use Edit tool)

# 3. Verify changes
git diff index.html

# 4. Commit
git add index.html
git commit -m "Descriptive message"

# 5. Push (with retry logic)
git push -u origin claude/claude-md-mi8mab6h0gp2e1tk-01DZBQz5Q9ikq7q2qcuo9TAH
```

## Deployment

### Hosting
This is a static HTML page that can be hosted on:
- GitHub Pages
- Netlify
- Vercel
- Any static hosting service
- Traditional web servers

### Configuration
- No build process required
- No server-side processing
- Direct deployment of index.html
- Ensure proper MIME types (text/html)

## Support and Contact

### Repository Owner
- GitHub: Ayoubbenderdouch
- Repository: -privacy-policy

### Application Contact
- Email: dinarchange@gmail.com
- Website: https://changedinar.online/

## Version History

### Current State
- **Files**: 2 (README.md, index.html)
- **Lines of Code**: ~223 lines in index.html
- **Last Updated**: 16/02/2025 (per document content)
- **Git Commits**:
  - 2528455: Add files via upload
  - caea05f: Initial commit

## Additional Notes for AI Assistants

### Context Awareness
- This is a **privacy policy page**, not the actual application
- The application is a mobile currency exchange app
- The page exists to fulfill legal requirements
- Changes should be conservative and legally sound

### Best Practices
1. **Always preserve legal accuracy** - when in doubt, ask user
2. **Maintain RGPD compliance** - this is critical for EU users
3. **Keep content simple** - users need to understand their rights
4. **Update dates consistently** - track when changes were made
5. **Test responsiveness** - many users view on mobile devices

### When Unsure
If you're uncertain about:
- **Legal implications** → Ask the user before proceeding
- **Translation accuracy** → Verify French legal terms
- **Contact information** → Confirm with user before changing
- **Structural changes** → Explain plan and get approval first

---

**This document was generated on**: 2025-11-21
**For**: AI assistants working with the -privacy-policy repository
**Purpose**: Provide comprehensive context for effective collaboration
