# aeo-demo-auto

## Project
AEO (AI-Friendly) demo template for the auto industry using HTML with Schema.org, llms.txt, FAQ, and AI-friendly markup.

## Conventions
- Use semantic HTML5 elements
- Include Schema.org structured data in JSON-LD format
- Add llms.txt for AI crawler compatibility
- Place FAQ in structured data + visible HTML
- Use accessible, screen-reader friendly markup

## Naming
- Use lowercase with hyphens for file names: `index.html`, `about-us.html`
- Use descriptive class names: `.vehicle-listing`, `.faq-item`
- Name JSON-LD files with `-schema` suffix

## Architecture
- Single-page or multi-page static HTML
- Schema.org data embedded inline or in separate JSON-LD files
- FAQ section with both visible content and structured data
- No JavaScript framework required; vanilla JS only if needed

## Commands
- No build commands — pure static HTML deployment
- Validate markup with W3C Validator
- Test structured data with Google Rich Results Test

## Do Not
- Do not remove Schema.org JSON-LD from templates
- Do not break llms.txt generation or inclusion
- Do not use non-semantic div soup
- Do not omit alt text on images
- Do not add unnecessary client-side frameworks