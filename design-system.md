# Stardust Design System

## Color System
The Stardust Design System uses a small and simple color palette to keep the interface consistent and easy to read.

- `--color-primary: #6c63ff`  
  This is the main accent color. It is used for the button background to draw attention to important actions.

- `--color-background: #f5f3ff`  
  This is the page background color. It gives the page a soft and calm appearance.

- `--color-surface: #ffffff`  
  This is used for surfaces such as the card background and button text. It helps content stand out clearly against the page background.

- `--color-text: #333333`  
  This is the main text color used throughout the page. It provides strong readability.

- `--color-border: #d9d4f5`  
  This is used for the card border to create separation without making the design feel heavy.

The color system was kept intentionally simple so it would be easier to maintain and more reusable across a small design system.

## Typography System
The design system uses two font families to create contrast between headings and body text.

- `--font-body: Arial, sans-serif`  
  This is used for body text because it is clean, simple, and easy to read.

- `--font-heading: Georgia, serif`  
  This is used for headings to give the page more personality and visual contrast.

### Font Sizes
- `--font-size-md: 1rem`  
  Used for paragraph text and button text.

- `--font-size-lg: 1.5rem`  
  Used for section headings and the card title.

- `--font-size-xl: 2rem`  
  Defined as part of the text scale.

- `--font-size-xxl: 3.5rem`  
  Used for the main page title so it stands out clearly from the rest of the content.

The typography system helps create hierarchy by making the main heading the largest, section headings medium-sized, and paragraph text smaller and more readable.

## Spacing Rules
The spacing system uses a consistent 8-point scale.

- `--space-1: 8px`
- `--space-2: 16px`
- `--space-3: 24px`

### Vertical Spacing
Vertical spacing is used between headings, paragraphs, sections, and components to keep the page from feeling crowded.

### Horizontal Spacing
Horizontal spacing is used inside the button and inside the card for padding.

Examples:
- Buttons use `var(--space-1)` for top and bottom padding
- Buttons use `var(--space-2)` for left and right padding
- Cards use `var(--space-2)` for inside padding
- Sections use `var(--space-3)` for spacing underneath each section

Using only three spacing values keeps the layout simple, consistent, and easier to understand.

## Component Guidelines

### Buttons
The button uses the primary color, surface color, spacing tokens, and font tokens.

#### Button Rules
- Background color uses `var(--color-primary)`
- Text color uses `var(--color-surface)`
- Font size uses `var(--font-size-md)`
- Padding uses `var(--space-1)` vertically and `var(--space-2)` horizontally
- Border radius is `8px`
- Shadow uses `var(--shadow)`

#### Button States
- Default state: purple background with white text
- Hover state: uses `opacity: 0.9`
- Focus state: uses a visible outline for accessibility

Buttons should be used for primary actions that need user attention.

### Cards
The card is used as a reusable content container.

#### Card Rules
- Background uses `var(--color-surface)`
- Border uses `var(--color-border)`
- Padding uses `var(--space-2)`
- Border radius is `8px`
- Shadow uses `var(--shadow)`
- Maximum width is `500px`

#### Card Content
- Card titles use the heading font and `var(--font-size-lg)`
- Card body text uses the base paragraph size

Cards should be used to group related content into a clean and readable block.

## Design Principles

### Consistency
The design system reuses the same colors, spacing values, and typography choices throughout the page. This makes the interface feel connected and easier to maintain.

### Accessibility
The design uses readable text colors, clear spacing, hover feedback, and a visible focus state for the button. These choices improve usability and help support accessibility.

### Clarity
The system was designed to be simple instead of overly decorative. The goal was to make the code easy to understand and the interface easy to scan.

## AI Feedback and Improvements
After reviewing the design system with AI, I made several improvements:

1. I simplified the spacing scale to only three spacing variables so the system would be easier to use consistently.
2. I increased the size of the main heading so the page would have stronger visual hierarchy.
3. I centered the layout and text so the page would feel more balanced.
4. I added a button focus state to improve accessibility.

These changes made the design system clearer, more consistent, and easier to explain.

## Reflection Questions

### How does defining design tokens improve your code?
Defining design tokens improves my code because it makes the design more consistent and easier to update. Instead of changing the same color, font, or spacing in multiple places, I can update one variable and have it apply across the whole design.

### What tradeoffs did you consider when choosing your color palette?
The main tradeoff was keeping the palette visually interesting while also keeping it simple. I wanted the page to have a soft and playful look, but I also wanted to avoid using too many colors so the design system would stay clear and reusable.

### How did AI critique influence your final design?
AI critique helped me simplify the spacing system, improve the heading hierarchy, and think more carefully about accessibility. It also helped me make the layout feel more balanced by centering the content and refining the styling choices.

### If you were building a full design, what would be the next components to add?
If I were expanding this into a larger design system, I would add input fields, navigation components, alerts, and badges. These are common interface elements that would benefit from the same reusable rules.