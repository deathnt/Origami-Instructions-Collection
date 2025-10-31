# Contributing to Origami Instructions Collection

Thank you for your interest in contributing to the Origami Instructions Collection! This project aims to create a comprehensive, open-source library of origami tutorials. Whether you're a beginner or an expert folder, your contributions are welcome!

## Table of Contents

- [File Organization](#file-organization)
- [Naming Conventions](#naming-conventions)
- [Markdown Formatting Standards](#markdown-formatting-standards)
- [Image Requirements](#image-requirements)
- [Tutorial Structure Template](#tutorial-structure-template)
- [Step-by-Step Workflow](#step-by-step-workflow-for-adding-tutorials)
- [Quality Guidelines](#quality-guidelines)
- [Review Process](#review-process)

---

## File Organization

### Folder Structure

All tutorials should be organized in the following directory structure:

```
tutorials/
├── beginner/
│   ├── crane/
│   │   ├── crane.md
│   │   └── images/
│   │       ├── step-01.jpg
│   │       ├── step-02.jpg
│   │       └── ...
│   └── boat/
│       ├── boat.md
│       └── images/
├── intermediate/
│   ├── rose/
│   │   ├── rose.md
│   │   └── images/
│   └── dragon/
│       ├── dragon.md
│       └── images/
└── advanced/
    ├── phoenix/
    │   ├── phoenix.md
    │   └── images/
    └── kusudama/
        ├── kusudama.md
        └── images/
```

### Difficulty Levels

- **beginner/**: Simple models with 10-15 steps, suitable for those new to origami
- **intermediate/**: Models with 15-30 steps, requiring some experience
- **advanced/**: Complex models with 30+ steps, requiring significant skill

---

## Naming Conventions

### Folder Names
- Use lowercase with hyphens for multi-word names
- Examples: `crane`, `jumping-frog`, `modular-box`

### File Names
- Tutorial file: Use the same name as the folder with `.md` extension
  - Example: `crane/crane.md`
- Image files: Use descriptive names with step numbers
  - Format: `step-XX.jpg` or `step-XX-description.jpg`
  - Examples: `step-01.jpg`, `step-05-valley-fold.jpg`, `final-result.jpg`

### No Special Characters
- Avoid spaces, special characters, or capital letters in file/folder names
- Use hyphens (`-`) instead of underscores or spaces

---

## Markdown Formatting Standards

### Headers
```markdown
# Model Name (H1 - Title only)
## Section Name (H2 - Main sections)
### Subsection (H3 - Sub-sections)
```

### Text Formatting
- **Bold** for emphasis: `**text**`
- *Italic* for origami terms: `*valley fold*`, `*mountain fold*`
- `Code` for measurements: `` `15cm x 15cm` ``

### Lists
```markdown
1. Ordered lists for step-by-step instructions
2. Second step
3. Third step

- Unordered lists for materials
- Or tips and notes
```

### Links and Images
```markdown
![Step description](images/step-01.jpg)
[External resource](https://example.com)
```

---

## Image Requirements

### Technical Specifications

- **Format**: JPEG (`.jpg`) or PNG (`.png`)
  - Use JPEG for photographs
  - Use PNG for diagrams or images requiring transparency
- **Resolution**: 1200px on the longest side (minimum 800px)
- **File Size**: Maximum 2MB per image (compress if necessary)
- **Aspect Ratio**: 4:3 or 1:1 preferred for consistency

### Image Quality Standards

- **Lighting**: Well-lit images with no harsh shadows
- **Focus**: Sharp, in-focus images showing clear fold lines
- **Background**: Clean, neutral background (white or light gray preferred)
- **Angle**: Consistent viewing angle across all steps
- **Hands**: Hands may be visible to demonstrate technique, but should not obstruct the model

### Image Naming Convention

```
step-01.jpg              // Basic step
step-02-valley-fold.jpg  // Step with description
step-15-detail.jpg       // Close-up detail
final-result-front.jpg   // Final model (front view)
final-result-side.jpg    // Final model (side view)
```

### Image Optimization

- Compress images using tools like:
  - [TinyJPG](https://tinyjpg.com/)
  - [ImageOptim](https://imageoptim.com/)
  - Command line: `imagemagick` or `jpegoptim`
- Ensure images are oriented correctly before uploading

---

## Tutorial Structure Template

Use the following template for all tutorial markdown files:

```markdown
# [Model Name]

![Final Result](images/final-result.jpg)

## Overview

**Difficulty**: [Beginner/Intermediate/Advanced]
**Estimated Time**: [XX minutes]
**Paper Required**: [e.g., 1 square sheet, 15cm x 15cm]
**Creator/Designer**: [Original designer name, if known]

## Description

[2-3 sentences describing the model, its characteristics, and any cultural or historical significance]

## Materials

- 1 square sheet of origami paper (15cm x 15cm recommended)
- [Any additional materials needed]

## Tips Before Starting

- [Tip 1: e.g., "Use paper with different colors on each side for easier learning"]
- [Tip 2: e.g., "Pre-crease diagonal folds for better accuracy"]
- [Tip 3]

## Instructions

### Step 1: [Brief description]
![Step 1](images/step-01.jpg)

[Detailed instructions for this step]

### Step 2: [Brief description]
![Step 2](images/step-02.jpg)

[Detailed instructions for this step]

[Continue with all steps...]

### Final Step: [Brief description]
![Final Result](images/final-result.jpg)

[Final shaping instructions and completion notes]

## Variations

- [Optional: Different ways to modify or enhance the model]
- [Different paper sizes or types]

## Troubleshooting

- **Problem**: [Common issue]
  - **Solution**: [How to fix it]
- **Problem**: [Another common issue]
  - **Solution**: [How to fix it]

## References

- [Optional: Links to original sources, videos, or related resources]
- Designer credit: [Name and link if available]

## Tags

`#animal` `#traditional` `#paper-crane` `#beginner-friendly`
```

---

## Step-by-Step Workflow for Adding Tutorials

### 1. Fork the Repository

```bash
# Click "Fork" button on GitHub
# Clone your fork
git clone https://github.com/YOUR-USERNAME/Origami-Instructions-Collection.git
cd Origami-Instructions-Collection
```

### 2. Create a New Branch

```bash
# Create a branch with a descriptive name
git checkout -b add-tutorial-crane
```

### 3. Create Tutorial Folder Structure

```bash
# Navigate to appropriate difficulty level
cd tutorials/beginner/

# Create model folder and images subfolder
mkdir -p crane/images
cd crane
```

### 4. Add Your Tutorial Content

- Create `crane.md` using the template above
- Add all images to the `images/` folder
- Ensure all images are properly named and optimized

### 5. Test Your Tutorial

- Preview your markdown file locally
- Verify all images load correctly
- Check for typos and formatting issues
- Ensure links work properly

### 6. Commit Your Changes

```bash
# Stage your files
git add .

# Commit with a descriptive message
git commit -m "Add beginner crane tutorial with 12 steps"
```

### 7. Push to Your Fork

```bash
git push origin add-tutorial-crane
```

### 8. Create a Pull Request

- Go to your fork on GitHub
- Click "New Pull Request"
- Fill out the PR template (see below)
- Submit for review

### Pull Request Template

```markdown
## Tutorial Information

- **Model Name**: [e.g., Traditional Crane]
- **Difficulty Level**: [Beginner/Intermediate/Advanced]
- **Number of Steps**: [e.g., 12]
- **Original Designer**: [Name or "Traditional"]

## Checklist

- [ ] Tutorial follows the standard template
- [ ] All images are optimized and under 2MB
- [ ] Images are properly named and organized
- [ ] Markdown formatting is correct
- [ ] Tutorial has been tested and reviewed locally
- [ ] All steps are clear and accurate
- [ ] Proper attribution provided for designer

## Additional Notes

[Any additional context or information about this tutorial]
```

---

## Quality Guidelines

### Content Quality

- **Accuracy**: All instructions must be tested and accurate
- **Clarity**: Use clear, concise language that beginners can understand
- **Completeness**: Include all necessary steps without skipping details
- **Attribution**: Always credit the original designer if known

### Writing Style

- Use active voice: "Fold the paper in half" (not "The paper should be folded")
- Be specific: "Fold the top corner down to meet the bottom edge" (not "Fold down")
- Use consistent terminology throughout
- Define special terms the first time they appear

### Common Origami Terms

- **Valley fold**: Fold towards you (creates a V-shaped valley)
- **Mountain fold**: Fold away from you (creates a peak)
- **Crease**: A fold that is then unfolded, leaving a line
- **Reverse fold**: Inside or outside fold that changes direction
- **Squash fold**: Fold that opens and flattens a pocket
- **Petal fold**: Combination of valley and mountain folds

### Image Quality Checklist

- [ ] Image is in focus and well-lit
- [ ] Paper and folds are clearly visible
- [ ] Consistent angle and distance across steps
- [ ] Clean background with no distractions
- [ ] File size is optimized (under 2MB)
- [ ] Image dimensions are appropriate (min 800px)

### Tutorial Completeness

- [ ] Includes overview and materials list
- [ ] All steps are numbered and have images
- [ ] Final result image is included
- [ ] Tips or troubleshooting section (if applicable)
- [ ] Proper attribution to designer
- [ ] Appropriate difficulty level assigned

---

## Review Process

### What to Expect

1. **Initial Review** (1-3 days)
   - Maintainers will review your PR for formatting and completeness
   - May request changes or improvements

2. **Content Verification** (2-5 days)
   - Community members may test your tutorial
   - Feedback provided on clarity and accuracy

3. **Final Approval**
   - Once approved, your tutorial will be merged
   - You'll be credited as a contributor!

### Review Criteria

- [ ] Follows file organization standards
- [ ] Uses correct naming conventions
- [ ] Meets markdown formatting requirements
- [ ] Images meet technical and quality standards
- [ ] Tutorial is complete and accurate
- [ ] Writing is clear and instructional
- [ ] Proper attribution included

### Responding to Feedback

- Be responsive to reviewer comments
- Make requested changes promptly
- Ask questions if feedback is unclear
- Update your PR branch with fixes:

```bash
# Make your changes
git add .
git commit -m "Address review feedback: improve step 5 clarity"
git push origin add-tutorial-crane
```

### After Your PR is Merged

- Your contribution will appear in the main repository
- You'll be listed as a contributor
- Consider adding more tutorials!
- Help review other contributors' submissions

---

## Code of Conduct

### Our Standards

- Be respectful and inclusive
- Provide constructive feedback
- Accept criticism gracefully
- Focus on what's best for the community

### Attribution and Copyright

- Only submit tutorials you have permission to share
- Credit original designers whenever possible
- For traditional models, note them as "Traditional"
- Do not submit copyrighted content without permission
- All contributions should be compatible with the repository's open-source license

---

## Need Help?

- **Questions?** Open an [issue](https://github.com/deathnt/Origami-Instructions-Collection/issues) with the "question" label
- **Bug reports?** Use the "bug" label when creating an issue
- **Feature requests?** Use the "enhancement" label

## Additional Resources

- [Markdown Guide](https://www.markdownguide.org/)
- [Origami Terminology](https://www.origami-resource-center.com/origami-terms.html)
- [GitHub Flow Guide](https://guides.github.com/introduction/flow/)

---

Thank you for contributing to the Origami Instructions Collection! Your efforts help make origami accessible to everyone. Happy folding! 🦢📄
