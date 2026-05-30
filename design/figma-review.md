# Figma Design Review

> Figma file URL → structured design review with feedback comments posted directly into Figma.

## Context

You need to review a UI/UX design in Figma and provide structured feedback. This skill reviews designs from an implementer's perspective — checking spacing, color contrast, grid alignment, component consistency, and interaction patterns — and writes feedback comments directly into the Figma file at the exact locations where issues exist. Closes the review loop without leaving Figma.

Useful for PMs reviewing designer output, eng managers checking implementation feasibility, and marketers reviewing landing page designs.

## Instructions

1. I will provide a Figma file URL (with a specific frame/page selected).

2. **Prerequisites check:**
   - Figma MCP connection is available
   - Figma Personal Access Token is set (`FIGMA_TOKEN` environment variable)
   - Figma desktop app is open with the target file

3. **Phase A — Basic design review** (automated checks):

   | Check | What to look for |
   |-------|-----------------|
   | Spacing | Consistent padding/margins, alignment to a spacing scale (4px/8px grid) |
   | Color contrast | WCAG AA compliance (4.5:1 for text, 3:1 for large text) |
   | Grid alignment | Elements snap to the layout grid, no off-grid outliers |
   | Typography | Consistent font sizes, weights, and line heights across the design |
   | Component consistency | Same UI element should look the same everywhere (buttons, inputs, cards) |
   | Sizing | Touch targets >= 44x44px, consistent icon sizes |

4. **Phase B — Implementation review** (contextual checks):

   | Check | What to look for |
   |-------|-----------------|
   | Data states | Does the design handle empty, loading, error, and overflow states? |
   | Edge cases | Long text truncation, missing avatars, zero-data scenarios |
   | Tables & lists | Column alignment, sort indicators, pagination, responsive behavior |
   | Forms | Validation states, error messages, required field indicators, tab order |
   | Interactions | Hover, focus, active, disabled states for interactive elements |
   | Permissions | Does the UI change based on user role? Are admin-only actions separated? |
   | Responsive | Will this layout work on smaller viewports? |

5. **Post feedback to Figma:**
   - For each issue found, post a comment directly in the Figma file at the relevant location
   - Format: `[Category] Issue description. Suggestion: ...`
   - Example: `[Spacing] Button padding is 6px, but the system uses 8px increments. Suggestion: change to 8px padding.`

6. **Produce a summary report:**

   | # | Category | Element | Issue | Severity |
   |---|----------|---------|-------|----------|
   | 1 | Spacing | Login button | 6px padding, system uses 8px | Low |
   | 2 | Contrast | Subtitle text | 3.2:1 ratio, needs 4.5:1 | High |
   | 3 | Missing state | Email input | No error state designed | Medium |

   Severity levels:
   - **High** — accessibility violation or broken interaction
   - **Medium** — inconsistency that will cause implementation questions
   - **Low** — polish item, can ship without fixing

7. If Figma MCP or FIGMA_TOKEN is not available, produce the review as a Markdown report without posting comments, and note that direct Figma commenting was skipped.

## Example

### Input

```
Review this Figma design: https://www.figma.com/file/abc123/Landing-Page?node-id=12:345
Focus on mobile responsiveness and form validation states.
```

### Output

**Design Review: Landing Page — Mobile & Form Focus**

| # | Category | Element | Issue | Severity | Figma comment posted |
|---|----------|---------|-------|----------|---------------------|
| 1 | Responsive | Hero section | Text is 48px — will overflow on 375px viewport | High | Yes |
| 2 | Form | Email input | No error state (invalid email, empty submit) | High | Yes |
| 3 | Form | Submit button | No disabled state while form is invalid | Medium | Yes |
| 4 | Spacing | CTA section | 12px gap between input and button, system uses 16px | Low | Yes |
| 5 | Contrast | Footer links | 3.8:1 ratio on gray background, needs 4.5:1 | Medium | Yes |

**Summary:** 2 high-severity issues (responsive overflow and missing error states), 2 medium, 1 low. Recommend addressing the form validation states before handoff to engineering — these will be the first thing QA flags.

**5 comments posted to Figma** at the relevant nodes.

---

## Source

Initial raw source: [shomtsm/figma-review-skill](https://github.com/shomtsm/figma-review-skill)
