Copyright 2024 Tina Kucina

Applying BEM Methodology in Our Project

The BEM (Block, Element, Modifier) methodology was fundamental in structuring our project, ensuring clarity, maintainability, and scalability. Here’s how we implemented it:

Key Blocks, Elements, and Modifiers

Header (.header)

.header__logo - the logo section.

.header__nav - navigation container.

.header__menu - unordered list of navigation links.

.header__item - individual navigation items.

.header__link - actual links within the navigation.

Modifiers:

.header--sticky - sticky version of the header.

Hero Section (.hero)

.hero__content - text-based content.

.hero__title - main heading.

.hero__text - supporting text.

.hero__image - image section.

Modifiers:

.hero--fullwidth - applies a full-width layout when needed.

Features Section (.features)

.features__list - container for feature items.

.features__item - single feature card.

.features__item-title - feature title.

.features__item-text - feature description.

.features__item-image - feature image.

Modifiers:

.features__item--highlighted - emphasizes a specific feature.

Testimonials (.testimonials)

.testimonials__list - container for testimonials.

.testimonial - individual testimonial block.

.testimonial__image - reviewer’s photo.

.testimonial__content - text content.

.testimonial__name - name of the reviewer.

Modifiers:

.testimonial--featured - highlights specific testimonials.

Call-to-Action (.cta)

.cta__title - CTA heading.

.cta__text - supporting text.

.cta__button - call-to-action button.

Modifiers:

.cta__button--primary - primary action button.

.cta__button--secondary - secondary button style.

By following BEM, we achieved:

Scalability: Each component can be easily extended or modified without affecting other parts.

Reusability: Components are independent and reusable across different sections.

Readability: Clear naming conventions make it easy to understand the structure.

Stack and Cover Layouts: Usage and Benefits

For layout structuring, we applied Stack and Cover models, ensuring usability and maintainability.

Stack Layout

We used the Stack layout where elements should be naturally arranged in a vertical column with consistent spacing:

Testimonials Section (.testimonials__list): Each testimonial is stacked with even spacing.

Feature List (.features__list): Features are arranged in a column-first approach before adjusting for larger screens.

Cover Layout

The Cover layout was essential in our Hero Section (.hero), ensuring content is vertically and horizontally centered with flexible padding. This layout helps with:

Maintaining Focus: The core message remains at the center regardless of screen size.

Responsive Design Without Media Queries: Adjusts naturally without explicit breakpoints.

styles/
│── base/
│   ├── _reset.scss  // Global resets
│   ├── _typography.scss  // Font styles
│── layout/
│   ├── _grid.scss  // Grid system
│   ├── _header.scss  // Header layout
│   ├── _footer.scss  // Footer layout
│── components/
│   ├── _button.scss  // Button styles
│   ├── _card.scss  // Card components
│   ├── _testimonials.scss  // Testimonials section
│── utilities/
│   ├── _variables.scss  // Color, typography variables
│   ├── _mixins.scss  // Reusable mixins
│── pages/
│   ├── _home.scss  // Homepage-specific styles
│   ├── _about.scss  // About page-specific styles


Advantages of this Structure:

Modularity: Each section is managed separately, making updates efficient.

Reusability: Components and utilities are reusable across different pages.

Scalability: New sections or styles can be added without modifying existing files.

Conclusion

This project was built with BEM for structure, Stack and Cover for layout, and SASS for maintainability. These best practices ensured clean, scalable, and reusable code, allowing for effortless updates and future expansions.