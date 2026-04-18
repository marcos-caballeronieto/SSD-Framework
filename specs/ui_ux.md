# UI/UX & Design System Specification

## 1. Visual Identity & Brand
*Define the "look and feel" to guide the Agent's CSS generation.*
- **Design Philosophy:** [e.g., Neubrutalism, Minimalist SaaS, Material Design 3, Retro-CGA]
- **Visual Vibe:** [e.g., High-contrast, playful, professional, dark-mode first]
- **Reference Theme:** [Link to Theme Factory skill or external style guide]

## 2. Design Tokens (Theme Factory Input)
*The Agent will use these as CSS variables or Tailwind constants.*
- **Color Palette:**
    - **Primary:** `[Hex Code]` (Main actions)
    - **Secondary:** `[Hex Code]` (Supporting elements)
    - **Background:** `[Hex Code]`
    - **Surface/Card:** `[Hex Code]`
    - **Status:** (Success: `[Hex]`, Warning: `[Hex]`, Error: `[Hex]`)
- **Typography:**
    - **Headings:** [e.g., Montserrat, Bold]
    - **Body:** [e.g., Inter, Regular, 16px]
    - **Code/Mono:** [e.g., Fira Code]
- **Spacing System:** [e.g., 4px base (Tailwind default), 8px grid]
- **Border Radius:** [e.g., 8px (Rounded), 0px (Sharp/Brutalist)]

## 3. Core Component Library
*Pre-define the components to ensure consistency across the app.*
- **Buttons:** [Describe states: Idle, Hover, Active, Disabled]
- **Inputs:** [Describe focus states and error styling]
- **Cards:** [Describe shadows, borders, and padding]
- **Navigation:** [e.g., Sidebar, Top Navbar, Bottom Tabs]

## 4. User Interaction & Flows
*How the user moves through the "Mission".*
- **Main Flow:** [e.g., Login -> Dashboard -> Action -> Feedback]
- **Micro-interactions:** [e.g., "Buttons should bounce slightly on click", "Fade-in transitions for page changes"]
- **Loading States:** [e.g., Skeleton loaders, progress bars]

## 5. Responsive Strategy
- **Mobile First:** [Yes/No]
- **Breakpoints:** [e.g., SM: 640px, MD: 768px, LG: 1024px]
- **Hidden Elements:** [Which features are hidden on small screens?]

## 6. Accessibility (a11y) & Usability
*Crucial for professional-grade AI development.*
- **Contrast Ratio:** [e.g., WCAG AA Standard (4.5:1)]
- **Navigation:** [e.g., Full keyboard navigation support (Tab-indexing)]
- **Screen Readers:** [Requirement for `aria-labels` on all interactive icons]

## 7. UI Constraints for Agents
- **No Mystery Icons:** Every icon must have a tooltip or a visible label.
- **Consistency:** If a design pattern is established in one feature, it must be reused in all others.
- **Asset Usage:** Use `Lucide Icons` (or similar) exclusively; do not fetch random images.