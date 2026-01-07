# Music Structure Visualizer

A static web visualization tool designed to analyze and represent the structural arrangement of musical compositions. This project translates musical time (bars/measures) into proportional visual blocks using CSS Flexbox logic.

## Project Overview

This tool solves the problem of visualizing song structures (Intro, Verse, Hook, Bridge) without needing complex audio software. It provides a clear, color-coded "map" of a track's arrangement, allowing producers and engineers to analyze the "Sonic DNA" of a song at a glance.

## Key Features

- **Proportional Visualization:** Uses CSS Flexbox (`flex-grow`) to mathematically represent the duration of each section. A 16-bar verse is visually exactly twice as long as an 8-bar hook.
- **Semantic Color Coding:** Distinct color palette for immediate identification of song sections (e.g., Red for Hooks, Blue for Verses).
- **Responsive Design:** Optimized for both desktop and mobile viewing. Text labels adapt or hide based on available screen real estate.
- **Lightweight Architecture:** Built with pure HTML5 and CSS3. No JavaScript frameworks or external dependencies required.
- **Modern Typography:** Implements 'Plus Jakarta Sans' for a clean, geometric aesthetic.

## Technical Implementation

The core logic relies on the CSS Flexible Box Layout. Each song is a container, and each section is a child element with a `flex` property corresponding to its musical length.

**Example Logic:**

```css
/* A standard 4-bar Intro */
.section-intro {
    flex: 4;
}

/* A standard 16-bar Verse */
.section-verse {
    flex: 16;
}
