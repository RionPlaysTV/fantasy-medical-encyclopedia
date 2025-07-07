<!-- Use this file to provide workspace-specific custom instructions to Copilot. For more details, visit https://code.visualstudio.com/docs/copilot/copilot-customization#_use-a-githubcopilotinstructionsmd-file -->

# Anatomica Fantastica - Copilot Instructions

This is a Jekyll-based fantasy medical encyclopedia website designed for GitHub Pages deployment.

## Project Structure
- `_species/` - Individual species medical entries in Markdown
- `_layouts/` - Jekyll layout templates
- `_config.yml` - Jekyll configuration
- `index.md` - Homepage
- `species.md` - Species index page
- `about.md` - About page

## Content Guidelines
When creating or editing species entries:

1. **Follow the established format** with proper front matter including title, layout, and lifespan
2. **Use consistent emoji headers** for each section (🧬, 📏, 🫀, 🩺, ✨, 🧪, 🥼, 🧂, 🌿, 📓)
3. **Maintain the scholarly but engaging tone** with occasional dry humor
4. **Include practical medical information** - dosages, emergency protocols, contraindications
5. **Respect cultural aspects** of each species' medical practices
6. **Cross-reference other species** when relevant for treatment comparisons

## Technical Notes
- All content must be valid Markdown for Jekyll processing
- Use Jekyll liquid tags for dynamic content (species listings, navigation)
- Maintain responsive design with CSS grid for species cards
- Optimize for GitHub Pages deployment (no custom plugins beyond Jekyll standards)

## Writing Style
- Semi-professional medical tone
- Include "Scholar's Notes" with first-person observations
- Add clinical warnings and emergency protocols
- Balance fantasy elements with medical realism
- Use species-appropriate terminology and avoid real-world medical references that break immersion
