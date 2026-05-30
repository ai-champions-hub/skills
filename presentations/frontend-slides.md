# Frontend Slides

> Topic or content → beautiful presentation slides as a single HTML file with zero dependencies.

## Context

You need a slide deck for a pitch, keynote, team meeting, or demo but don't want to wrestle with PowerPoint or Google Slides. This skill generates stunning HTML/CSS presentations as a single self-contained file — no dependencies, no build step, no framework. Just open the HTML file in a browser and present. Supports converting existing PowerPoint files to HTML as well.

Also supports deploying to Vercel and exporting to PDF.

## Instructions

1. I will describe what I need: the topic, audience, key points, and desired vibe. I may also provide a PowerPoint file to convert.

2. **Detect the mode:**
   - **New presentation** — create from scratch based on my content
   - **PPT conversion** — convert an existing PowerPoint to HTML
   - **Enhancement** — improve an existing HTML presentation

3. **Content discovery** (for new presentations):
   - What is the presentation about?
   - Who is the audience?
   - How many slides (suggest a range based on content)?
   - What's the key takeaway the audience should leave with?
   - Any specific data, quotes, or images to include?

4. **Style discovery:**
   - Generate 2-3 visual style previews as mini HTML files (3 slides each)
   - Let me choose the direction before building the full deck
   - Available style presets include: minimal, corporate, bold, editorial, dark, neon, gradient, retro, nature, tech, academic, creative

5. **Generate the presentation:**
   - Single HTML file with all CSS/JS inline
   - Fixed 16:9 aspect ratio (1920x1080 viewport)
   - Keyboard navigation (arrow keys, space bar)
   - Smooth slide transitions
   - Responsive text sizing
   - Print-friendly (Ctrl+P exports cleanly)

6. **Design rules:**
   - One idea per slide
   - Maximum 6 lines of text per slide (preferably fewer)
   - High contrast text on backgrounds
   - Generous whitespace
   - Consistent typography hierarchy (title, subtitle, body, caption)
   - Animations should be subtle and purposeful, not distracting
   - No clip art, no stock photo placeholders, no SmartArt

7. **Anti-AI-slop rules:**
   - No generic gradient backgrounds unless specifically requested
   - No "futuristic" neon themes by default
   - No decorative elements that don't serve the content
   - Typography and whitespace do the heavy lifting
   - Every visual element should earn its place

8. **Slide types available:**
   - Title slide (with subtitle and author)
   - Content slide (text + optional visual)
   - Data slide (chart, table, or key metrics)
   - Quote slide
   - Image slide (full-bleed or split)
   - Comparison slide (two columns)
   - Timeline slide
   - Section divider
   - Thank you / Q&A slide

9. **Delivery options:**
   - Save as `.html` file (default — works offline, zero dependencies)
   - Deploy to Vercel (`vercel deploy`) for a shareable URL
   - Export to PDF (Ctrl+P in browser, or use a headless browser)

## Example

### Input

```
Create a 10-slide pitch deck for an AI writing assistant startup. 
Audience: investors at a seed round pitch. 
Key points: $2M ARR, 40% MoM growth, 12K users, team of 6 ex-Google engineers.
Style: clean and minimal, dark background.
```

### Output

*(A single HTML file with 10 slides: title, problem, solution, demo, traction, market size, business model, team, ask, and closing. Dark minimal style, 16:9, keyboard navigation, all inline.)*

---

## Source

Initial raw source: [zarazhangrui/frontend-slides](https://github.com/zarazhangrui/frontend-slides)
