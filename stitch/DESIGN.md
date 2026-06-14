---
name: StackLens Canary Utility
colors:
  surface: '#fcf8fa'
  surface-dim: '#dcd9db'
  surface-bright: '#fcf8fa'
  surface-container-lowest: '#ffffff'
  surface-container-low: '#f6f3f5'
  surface-container: '#f0edef'
  surface-container-high: '#eae7e9'
  surface-container-highest: '#e4e2e4'
  on-surface: '#1b1b1d'
  on-surface-variant: '#45464d'
  inverse-surface: '#303032'
  inverse-on-surface: '#f3f0f2'
  outline: '#76777d'
  outline-variant: '#c6c6cd'
  surface-tint: '#565e74'
  primary: '#000000'
  on-primary: '#ffffff'
  primary-container: '#131b2e'
  on-primary-container: '#7c839b'
  inverse-primary: '#bec6e0'
  secondary: '#735c00'
  on-secondary: '#ffffff'
  secondary-container: '#fed01b'
  on-secondary-container: '#6f5900'
  tertiary: '#000000'
  on-tertiary: '#ffffff'
  tertiary-container: '#271901'
  on-tertiary-container: '#98805d'
  error: '#ba1a1a'
  on-error: '#ffffff'
  error-container: '#ffdad6'
  on-error-container: '#93000a'
  primary-fixed: '#dae2fd'
  primary-fixed-dim: '#bec6e0'
  on-primary-fixed: '#131b2e'
  on-primary-fixed-variant: '#3f465c'
  secondary-fixed: '#ffe083'
  secondary-fixed-dim: '#eec200'
  on-secondary-fixed: '#231b00'
  on-secondary-fixed-variant: '#574500'
  tertiary-fixed: '#fcdeb5'
  tertiary-fixed-dim: '#dec29a'
  on-tertiary-fixed: '#271901'
  on-tertiary-fixed-variant: '#574425'
  background: '#fcf8fa'
  on-background: '#1b1b1d'
  surface-variant: '#e4e2e4'
typography:
  headline-lg:
    fontFamily: Inter
    fontSize: 24px
    fontWeight: '700'
    lineHeight: 32px
    letterSpacing: -0.02em
  headline-md:
    fontFamily: Inter
    fontSize: 18px
    fontWeight: '600'
    lineHeight: 24px
    letterSpacing: -0.01em
  body-md:
    fontFamily: Inter
    fontSize: 14px
    fontWeight: '400'
    lineHeight: 20px
  body-sm:
    fontFamily: Inter
    fontSize: 12px
    fontWeight: '400'
    lineHeight: 16px
  data-mono:
    fontFamily: JetBrains Mono
    fontSize: 13px
    fontWeight: '500'
    lineHeight: 18px
  label-caps:
    fontFamily: Inter
    fontSize: 11px
    fontWeight: '700'
    lineHeight: 14px
    letterSpacing: 0.05em
rounded:
  sm: 0.125rem
  DEFAULT: 0.25rem
  md: 0.375rem
  lg: 0.5rem
  xl: 0.75rem
  full: 9999px
spacing:
  unit: 4px
  container-padding: 16px
  gutter: 12px
  row-height-compact: 32px
  row-height-standard: 44px
---

## Brand & Style
The design system is engineered for high-stakes operational environments where information density and precision are paramount. The aesthetic is **Industrial Minimalism**, prioritizing utility over ornamentation. It is designed for engineers and system operators who require a deterministic interface that minimizes cognitive load during rapid data parsing.

The visual language is characterized by:
- **High Information Density:** Compact spacing and reduced vertical rhythms to maximize on-screen data.
- **Monotech Logic:** A structural approach to layout where every pixel serves a functional purpose, utilizing subtle borders rather than shadows to define boundaries.
- **Operational Clarity:** High-contrast status indicators that draw immediate attention to system anomalies without creating visual noise.

## Colors
The palette, "Monotech," uses a professional foundation of deep navies and cool slates to provide a neutral backdrop for critical system data.

- **Primary (#0F172A):** Used for structural elements, navigation, and primary headers. It represents stability and authority.
- **Canary Accent (#FACC15):** Reserved for "Warning" states, system alerts, and active "Canary" deployment indicators. It is the primary tool for visual hierarchy in dense views.
- **Status Indicators:** Emerald (#10B981) and Rose (#F43F5E) are used strictly for binary Success/Error reporting to ensure immediate recognition of system health.
- **Neutral Scale:** Utilizes a range of slates for borders and secondary text to maintain a clean, layered look without relying on shadows.

## Typography
The typography strategy leverages two distinct families to separate narrative intent from technical data.

- **Inter:** The primary workhorse for interface labels, navigation, and headers. Its high x-height ensures legibility even at the compact scales required for high-density dashboards.
- **JetBrains Mono:** Used exclusively for data points, log outputs, metrics, and technical values. The monospaced nature allows for easier vertical scanning of numbers and IDs in tabular layouts.

**Scale Philosophy:** Sizes are kept intentionally small (peaking at 24px) to accommodate more information per viewport. Capitalization is used for metadata labels to create a clear "Property: Value" distinction.

## Layout & Spacing
This design system utilizes a **Fixed Grid** philosophy built on a 4px baseline.

- **Grid:** A 12-column layout for desktop views with fixed 16px margins and 12px gutters. 
- **Density:** We employ a "Compact First" approach. Standard table rows are 32px in height to ensure maximum data visibility.
- **Reflow:**
  - **Desktop (1280px+):** Full multi-pane dashboard layout with persistent sidebar.
  - **Tablet (768px - 1279px):** Sidebar collapses to icons; charts scale fluidly.
  - **Mobile (<767px):** Data tables convert to card-based list views; primary navigation moves to a bottom-bar or hamburger menu.

## Elevation & Depth
Depth is communicated through **Tonal Layering and Borders** rather than traditional shadows. This maintains the "Industrial" aesthetic and ensures clarity in complex layouts.

- **Base Layer:** The application background uses a subtle Slate-50 (#F8FAFC).
- **Surface Layer:** Containers and cards use a pure White background with a 1px solid border (#E2E8F0).
- **Active State:** To indicate focus or selection, use the Canary Yellow as a 2px left-side border accent rather than a drop shadow.
- **Dividers:** Use 1px borders to separate table rows and sidebar sections, maintaining a strict grid feel.

## Shapes
The shape language is "Soft-Industrial." While 90-degree corners feel too aggressive, a standard rounded corner feels too consumer-focused. This design system uses a strict **4px (0.25rem)** radius for all standard UI components.

- **Containers/Cards:** 4px radius.
- **Buttons/Inputs:** 4px radius.
- **Status Badges:** 2px radius (near-sharp) to distinguish them from interactive buttons.
- **Checkboxes:** 2px radius.

## Components

- **Buttons:** 
  - *Primary:* Solid Deep Navy (#0F172A) with white text. High contrast, sharp focus.
  - *Secondary:* Ghost style with 1px border.
  - *Warning/Canary:* Solid Canary Yellow with black text—used only for critical overrides or deployments.
- **Data Tables:** The core of the system. Use alternating row fills (Zebra striping) in very faint grey. Headers are uppercase `label-caps`. Technical values use `data-mono`.
- **Status Badges:** Compact, rectangular shapes. Use a "Subtle-Fill" approach (e.g., light green background with dark green text) to avoid overwhelming the user, except for 'Critical' states which use solid fills.
- **Input Fields:** Inset appearance with 1px borders. Focused state uses a 1px solid Primary border with no outer glow.
- **Utility Bar:** A persistent top-bar containing system-wide "Canary Health" toggles and environment switchers, styled in Primary navy to anchor the visual weight.