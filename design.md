# Personal Website — Design System

**Design Direction:** Contemporary Cinema\
**Version:** 1.0\
**Status:** Approved design specification. Prototype C implementation and validation are pending.

See [Design Exploration](design-exploration.md) for the earlier candidates and the selection of Prototype C.

## 1. Design Vision

A personal website experienced as an evolving collection of cinematic chapters rather than a conventional portfolio.

The website should reflect curiosity, individuality, professional depth, and an appreciation for everyday life.

Its visual identity combines contemporary typography, warm cinematic colors, personal photography, editorial composition, and thoughtful motion.

**Cinematic, but effortless. Personal, but professional. Expressive, but restrained.**

## 2. Creative Influences

The design draws inspiration from the following creative directions:

- **Cinematic Editorial:** Expressive typography, vintage cinematic colors, and the opening title cards of *Hacks*.
- **Personal Archive:** Personal collections, memories, photography, journals, and everyday experiences.
- **Epic Exploration:** Expansive landscapes, curiosity, discovery, and the cinematic atmosphere of *The Odyssey*.
- **Urban Cinematic:** Contemporary city life, visual energy, and the cinematic language of *Spider-Man: Brand New Day*.
- **Cinematic Minimalism:** Spatial depth, restrained composition, and the atmospheric storytelling of *Interstellar*.

These references should inform the visual language rather than be directly reproduced.

The selected direction is a synthesis of these influences, not an imitation of any individual reference.

## 3. Core Design Principles

### Clarity

Prioritize readability, intuitive navigation, and clear visual hierarchy over decorative complexity.

### Character

Create a recognizable visual identity through typography, color, photography, and composition. Avoid generic portfolio templates and excessive decorative effects.

### Storytelling

Present personal and professional experiences as meaningful chapters of an ongoing life story.

### Authenticity

Prioritize original personal photography, genuine experiences, and individual perspectives.

### Restraint

Use color, animation, and sound intentionally. Every visual or interactive element should serve a meaningful purpose.

### Longevity

Build a flexible design system that can evolve alongside new interests, projects, experiences, and professional development.

## 4. Color System

The website uses a light-first visual identity based on the Cinematic Editorial palette.

### Primary Colors

| Token | Color | HEX | Usage |
|---|---|---|---|
| `color-background` | Cream White | `#F5EFE4` | Primary page background |
| `color-text` | Charcoal | `#262A30` | Primary text and headings |
| `color-accent` | Brick Red | `#A64635` | Links, highlights, key actions, and selected typography |

### Secondary Colors

| Token | Color | HEX | Usage |
|---|---|---|---|
| `color-secondary` | Vintage Blue | `#294E75` | Chapter accents and supporting visuals |
| `color-tertiary` | Amber Gold | `#D3AB69` | Occasional decorative details |
| `color-text-muted` | Warm Gray | `#69645C` | Supporting text and metadata |
| `color-border` | Warm Stone | `#D8D0C4` | Dividers and subtle boundaries |

### Color Usage

- Maintain a predominantly light appearance.
- Use Brick Red with moderate intensity.
- Reserve accent colors for meaningful visual emphasis.
- Avoid excessive gradients, saturated backgrounds, and competing accent colors.
- Allow individual chapters to introduce secondary colors while maintaining the shared global palette.
- Validate text and interactive element contrast against WCAG 2.2 AA requirements.

The three primary colors are selected design decisions. Secondary and utility colors may be refined during implementation.

## 5. Typography

Typography is a primary element of the website's visual identity.

### Font Families

**Headings:** Space Grotesk

**Body and interface text:** Inter

**Chinese text:** Noto Sans SC, with appropriate system font fallbacks.

### Typography Scale

| Role | Size | Weight | Line Height |
|---|---:|---:|---:|
| Display | 64px | 700 | 1.05 |
| H1 | 43px | 700 | 1.15 |
| H2 | 32px | 700 | 1.2 |
| H3 | 24px | 600 | 1.3 |
| H4 | 20px | 600 | 1.4 |
| Body Large | 18px | 400 | 1.65 |
| Body | 16px | 400 | 1.65 |
| Caption | 12px | 400 | 1.5 |
| Label | 12px | 600 | 1.4 |

### Typography Rules

- Use Space Grotesk Bold as the signature display typeface.
- Use Inter for reading comfort, navigation, and professional content.
- Use zero letter spacing as the default for primary headings.
- Apply additional letter spacing selectively to small editorial labels.
- Use responsive typography for different viewport sizes.
- Preserve a clear hierarchy without excessive variations in font size or weight.
- Keep long-form reading content within approximately 60–75 characters per line.
- Self-host appropriately licensed font files to reduce external dependencies and improve accessibility across regions.

The selected heading reference size is 43px. The broader scale is an initial implementation specification.

## 6. Layout and Composition

### Global Layout

The website should use spacious editorial composition with intentional whitespace and a balanced relationship between typography and photography.

Recommended initial layout values:

- Desktop: 12-column grid.
- Tablet: 8-column grid.
- Mobile: 4-column grid.
- Maximum content width: 1440px.
- Reading content width: approximately 720px.
- Desktop page margins: 64–80px.
- Tablet page margins: 32–48px.
- Mobile page margins: 20–24px.

### Spacing System

Use a consistent 4px-based spacing scale:

`4 / 8 / 12 / 16 / 24 / 32 / 48 / 64 / 96 / 128`

Favor generous spacing between major sections and consistent spacing within related content groups.

### Composition Rules

- Balance typography and photography.
- Use whitespace as an intentional design element.
- Favor editorial layouts over dashboard-style card grids.
- Use asymmetric compositions selectively.
- Maintain clear alignment and predictable reading order.
- Prefer subtle borders and restrained corner radii.
- Avoid excessive shadows, glassmorphism, and decorative containers.

## 7. Homepage

### Selected Prototype

**Prototype C — A Life in Chapters**

The homepage combines the expressive typography of the Title Sequence layout with the expansive photography of the Cinematic Opening layout.

### Homepage Structure

1. Minimal header and navigation.
2. Editorial introduction and signature headline.
3. Wide cinematic photography.
4. Two primary chapter entrances:
   - Personal Life
   - Professional Experience
5. Selected stories, projects, or recent discoveries.
6. Minimal footer.

The homepage should establish a personal identity without overwhelming visitors with information.

The introductory copy and featured photography should remain independently editable.

## 8. Adaptive Chapter System

All chapters share the same foundational typography, colors, spacing, navigation, and interaction principles.

Individual chapters may adapt their composition, supporting colors, photography, and motion to reflect their content.

| Chapter | Visual Direction |
|---|---|
| Homepage | Cinematic Editorial |
| Personal Life | Personal Archive |
| Travel & Photography | Epic Exploration |
| Everyday Life | Warm Editorial Archive |
| Film & Culture | Urban Cinematic |
| Professional Experience | Modern Editorial |

These chapter names and structures may evolve with the website's information architecture.

Personal Life pages may offer richer visual storytelling and more expressive motion.

Professional Experience pages should prioritize clarity, credibility, efficient navigation, and restrained interaction.

## 9. Photography and Visual Assets

Personal photography is the preferred source of visual content.

### Photography Principles

- Prioritize original photographs taken by the website owner.
- Select images for their atmosphere, personal significance, and storytelling value.
- Favor natural light, authentic moments, urban environments, landscapes, and everyday details.
- Preserve natural photographic character.
- Avoid generic stock photography whenever possible.
- Avoid excessive filters and artificial cinematic effects.
- Use AI-generated or third-party assets only when intentionally selected and appropriately authorized.

### Image Presentation

Recommended aspect ratios:

- Cinematic hero: 21:9 or 16:9.
- Editorial photography: 4:3 or 3:2.
- Portrait photography: 3:4.
- Archive collections: flexible ratios within a consistent composition.

Images should include appropriate alternative text, responsive sizing, and optimized loading.

## 10. Motion and Interaction

### Selected Motion Direction

**Cinematic Rhythm**

Motion should create a sense of cinematic storytelling without interfering with usability.

### Approved Interaction Patterns

- **Staggered Title Reveal:** Introduce headings and supporting content in a carefully paced sequence.
- **Cinematic Image Reveal:** Reveal hero photography through subtle masking or progressive transitions.
- **Chapter Transition:** Provide smooth transitions between major website chapters.
- **Editorial Micro-interactions:** Use subtle underline animations, arrow movement, and responsive hover states.
- **Living Photography:** Introduce subtle environmental movement, such as clouds, water, shadows, or steam.
- **Scroll-triggered Storytelling:** Gradually reveal content during natural scrolling.
- **Ambient Sound:** Provide optional sound and music experiences.

### Motion Timing

| Interaction | Recommended Duration |
|---|---:|
| Homepage opening sequence | 800–1200ms |
| Chapter transition | 250–450ms |
| Micro-interactions | 150–250ms |
| Scroll-triggered reveal | 300–500ms |
| Image hover transition | 200–350ms |

Use natural easing curves and avoid abrupt or mechanical movement.

Recommended easing:

`cubic-bezier(0.22, 1, 0.36, 1)`

### Opening Sequence

Play the full cinematic opening once per browsing session.

Subsequent navigation back to the homepage should use shorter transitions rather than replaying the entire opening.

Navigation and essential content must remain available without waiting for the animation to finish.

### Adaptive Motion

- Personal Life: expressive but restrained cinematic motion.
- Professional Experience: minimal, functional motion.
- Mobile: lightweight and performance-conscious motion.

### Motion Restrictions

- No scroll hijacking.
- No mandatory splash screens.
- No custom cursor effects by default.
- No excessive parallax.
- No distracting repetitive animations.
- No animations that delay access to content.
- Support the `prefers-reduced-motion` system preference.
- Provide a way to pause persistent decorative motion.

## 11. Sound Experience

Sound is an optional layer of the website experience.

- Sound must be disabled by default.
- Visitors may explicitly enable or disable audio.
- Provide accessible playback, pause, and mute controls.
- Maintain the visitor's sound preference during navigation.
- Audio must not interfere with reading or professional content.
- Use only appropriately licensed, original, or otherwise authorized audio assets.
- The website must remain fully functional without sound.

## 12. Navigation and Language

The website should support two primary content directions:

- Personal Life
- Professional Experience

Navigation should be minimal, predictable, and accessible.

### Language

- English is the default website language.
- Provide an easily discoverable Chinese language switch.
- Preserve the selected language during navigation.
- Maintain visual consistency across both languages.
- Adapt text wrapping and spacing to the requirements of Chinese typography.
- Avoid embedding important text directly into images.

## 13. Components

Develop reusable components that follow the shared design system.

Core components include:

- Global header and navigation.
- Language switch.
- Cinematic hero.
- Editorial section heading.
- Chapter entrance.
- Photography gallery.
- Journal entry.
- Timeline.
- Travel map.
- Project showcase.
- Article layout.
- Audio controls.
- Footer.

Components should support chapter-specific variations without duplicating the underlying design system.

## 14. Responsive Design

The website must provide a coherent experience across desktop, tablet, and mobile devices.

Initial breakpoint references:

- Mobile: below 768px.
- Tablet: 768px–1023px.
- Desktop: 1024px and above.

Responsive behavior should include:

- Fluid typography and spacing.
- Simplified mobile compositions.
- Responsive photography and appropriate image cropping.
- Touch-friendly interactive elements.
- No horizontal overflow.
- No essential interaction that depends exclusively on hovering.

Mobile experiences should preserve the website's identity rather than simply shrink desktop layouts.

## 15. Accessibility and Performance

Target WCAG 2.2 AA accessibility.

### Accessibility

- Semantic HTML.
- Keyboard-accessible navigation.
- Visible focus indicators.
- Meaningful image alternative text.
- Sufficient text contrast.
- Reduced-motion support.
- Accessible audio controls.
- Correct language attributes.
- Clear and predictable interaction states.

### Performance

- Optimize image dimensions and file formats.
- Lazy-load non-critical media.
- Prioritize above-the-fold content.
- Self-host and optimize font assets.
- Avoid unnecessary animation libraries and dependencies.
- Prefer lightweight CSS and native browser capabilities where practical.
- Ensure essential content remains accessible if animations fail.

Target good Core Web Vitals under representative mobile conditions.

## 16. Design Governance

This document serves as the primary visual design reference for the personal website.

When implementing new pages or features:

1. Follow the established design tokens and typography system.
2. Reuse existing components before creating new ones.
3. Preserve the selected visual direction.
4. Adapt layouts to content without introducing unnecessary stylistic fragmentation.
5. Validate accessibility, responsiveness, and performance.
6. Document significant design decisions and deviations.

New visual directions may be explored independently before being incorporated into the primary design system.

## 17. Implementation Validation

Validate the following during Prototype C implementation:

- Actual Space Grotesk and Inter typography.
- English and Chinese layouts.
- Color contrast and interactive states.
- Homepage composition using original personal photography.
- Motion timing and reduced-motion behavior.
- Desktop, tablet, and mobile layouts.
- Audio compatibility and playback permissions.
- Real-world website performance.

Adjust implementation parameters where necessary while preserving the selected design direction.

## 18. Design Philosophy

The website is not a finished portrait.

It is an evolving record of a life — its places, passions, work, ideas, and discoveries.

Every design decision should contribute to an experience that feels clear, authentic, thoughtful, and unmistakably personal.
