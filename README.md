# Katherine Lopez — Certified Swim Instructor Portfolio

A polished, professional, mobile-first one-page static website built with Astro for Katherine Lopez, a Red Cross WSI certified swimming instructor.

## Features

- Astro static-first site
- Component-based architecture
- Plain global CSS, no Bootstrap
- Mobile-first responsive layout
- Accessible semantic markup
- SEO title, meta description, and Open Graph basics
- Toggleable future sections for scheduling and an AI assistant
- Static contact form ready to connect to Netlify Forms, Formspree, or another service

## Project Structure

```text
src/
  components/
    Header.astro
    Hero.astro
    About.astro
    LessonTypes.astro
    WhyChooseKatherine.astro
    ServiceArea.astro
    LessonLocations.astro
    HowItWorks.astro
    SchedulingSection.astro
    AiAssistantSection.astro
    ContactForm.astro
    Footer.astro
  layouts/
    BaseLayout.astro
  pages/
    index.astro
  styles/
    global.css
```

## Setup

Install dependencies:

```bash
npm install
```

Start the development server:

```bash
npm run dev
```

Build for production:

```bash
npm run build
```

Preview the production build:

```bash
npm run preview
```

## Feature Flags

The scheduling and AI assistant sections are included as components but hidden by default in `src/pages/index.astro`:

```js
const showSchedulingSection = false;
const showAiAssistantSection = false;
```

Set either flag to `true` to render the corresponding placeholder section.

## Contact Form

The contact form is static by default. To make it functional, connect it to a form service such as:

- Netlify Forms
- Formspree
- Basin
- A custom API endpoint

For Netlify Forms, you can add the appropriate `data-netlify="true"` attributes and configure the deployment on Netlify.
