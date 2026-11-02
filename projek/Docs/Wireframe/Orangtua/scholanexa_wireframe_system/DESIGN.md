---
name: ScholaNexa Wireframe System
colors:
  surface: '#f7f9fd'
  surface-dim: '#d8dade'
  surface-bright: '#f7f9fd'
  surface-container-lowest: '#ffffff'
  surface-container-low: '#f2f4f8'
  surface-container: '#eceef2'
  surface-container-high: '#e6e8ec'
  surface-container-highest: '#e0e2e6'
  on-surface: '#191c1f'
  on-surface-variant: '#45464c'
  inverse-surface: '#2d3134'
  inverse-on-surface: '#eff1f5'
  outline: '#76777d'
  outline-variant: '#c6c6cd'
  surface-tint: '#575e70'
  primary: '#000000'
  on-primary: '#ffffff'
  primary-container: '#141b2b'
  on-primary-container: '#7d8497'
  inverse-primary: '#c0c6db'
  secondary: '#585f6c'
  on-secondary: '#ffffff'
  secondary-container: '#dce2f3'
  on-secondary-container: '#5e6572'
  tertiary: '#000000'
  on-tertiary: '#ffffff'
  tertiary-container: '#261906'
  on-tertiary-container: '#968065'
  error: '#ba1a1a'
  on-error: '#ffffff'
  error-container: '#ffdad6'
  on-error-container: '#93000a'
  primary-fixed: '#dce2f7'
  primary-fixed-dim: '#c0c6db'
  on-primary-fixed: '#141b2b'
  on-primary-fixed-variant: '#404758'
  secondary-fixed: '#dce2f3'
  secondary-fixed-dim: '#c0c7d6'
  on-secondary-fixed: '#151c27'
  on-secondary-fixed-variant: '#404754'
  tertiary-fixed: '#f9debf'
  tertiary-fixed-dim: '#dcc2a4'
  on-tertiary-fixed: '#261906'
  on-tertiary-fixed-variant: '#55442d'
  background: '#f7f9fd'
  on-background: '#191c1f'
  surface-variant: '#e0e2e6'
typography:
  headline-lg:
    fontFamily: Inter
    fontSize: 32px
    fontWeight: '700'
    lineHeight: 40px
  headline-lg-mobile:
    fontFamily: Inter
    fontSize: 24px
    fontWeight: '700'
    lineHeight: 32px
  headline-md:
    fontFamily: Inter
    fontSize: 20px
    fontWeight: '600'
    lineHeight: 28px
  headline-sm:
    fontFamily: Inter
    fontSize: 18px
    fontWeight: '600'
    lineHeight: 24px
  title-md:
    fontFamily: Inter
    fontSize: 16px
    fontWeight: '600'
    lineHeight: 22px
  body-lg:
    fontFamily: Inter
    fontSize: 16px
    fontWeight: '400'
    lineHeight: 24px
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
  label-lg:
    fontFamily: Inter
    fontSize: 14px
    fontWeight: '600'
    lineHeight: 20px
  label-md:
    fontFamily: Inter
    fontSize: 12px
    fontWeight: '500'
    lineHeight: 16px
  label-sm:
    fontFamily: Inter
    fontSize: 11px
    fontWeight: '500'
    lineHeight: 14px
rounded:
  sm: 0.25rem
  DEFAULT: 0.5rem
  md: 0.75rem
  lg: 1rem
  xl: 1.5rem
  full: 9999px
spacing:
  gutter: 1rem
  margin: 1rem
  space-xs: 0.25rem
  space-sm: 0.5rem
  space-md: 1rem
  space-lg: 1.5rem
  space-xl: 2rem
---

## Brand & Style

This design system is built specifically for low-fidelity wireframing and prototyping of Indonesian high school (SMA/SMK/MA) academic management tools. Its primary objective is structural clarity, information architecture validation, and ergonomic testing without visual bias.

The aesthetic follows an intentional, blueprint-like wireframe discipline:
- **Strictly Non-Chromatic**: Absolute elimination of hue to focus stakeholder feedback on hierarchy, layout, and task flows rather than branding decisions.
- **Architectural Minimalism**: Layouts communicate through container density, line weight, and clear typographic scale rather than decorative embellishments.
- **Indonesian Context-First**: Text lengths, labels, and interaction verbs account natively for Bahasa Indonesia structures (e.g., *Tugas Mendatang*, *Nilai Rapor*, *Jadwal Pelajaran*, *Presensi Siswa*).
- **Tactile Accessibility**: Optimized for varied low-to-mid-tier Android mobile hardware common among Indonesian students, mandating strict minimum touch targets and robust contrast.

## Colors

The palette is strictly achromatic, leveraging the 5 defined tone tiers to express hierarchy, interaction states, and placeholder elements without color-tinted affordances:

- **Near-Black (`#111827`)**: Base typography, high-priority icons, primary button solid fills, and active boundary states.
- **Dark Gray (`#374151`)**: Secondary labels, section headers, unselected high-contrast indicators, and active borders.
- **Mid Gray (`#6B7280` / `#9CA3AF`)**: 
  - `#6B7280`: Supporting descriptive text, structural wireframe diagonal guides ('X'), and inactive controls.
  - `#9CA3AF`: Form input outlines, placeholder text (*teks petunjuk*), disabled components, and decorative divider strokes.
- **Light Gray (`#E5E7EB` / `#F3F4F6`)**:
  - `#E5E7EB`: Primary structural borders, card outlines, table gridlines, and disabled fill states.
  - `#F3F4F6`: Card surface fills, input background states, skeleton box placeholders, and table header rows.
- **White (`#FFFFFF`)**: Base screen canvas background and contrasting content fills on elevated cards.

## Typography

Inter serves across all typography roles to ensure clean, utilitarian readability on high-density data tables, subject lists, and schedules. 

- **Language Adaptations**: Indonesian phrases tend to be 15–25% longer than their English equivalents (e.g., *Submit* vs *Kirimkan Tugas*, *Settings* vs *Pengaturan Akun*). Line heights are defensively budgeted to prevent accidental clipping on tight mobile viewports.
- **Hierarchy Mapping**:
  - `headline-lg-mobile` & `headline-md`: Used for screen titles (*Beranda Siswa*, *Detail Nilai*) and modular headers.
  - `title-md`: Card headlines and list item headings (*Matematika Wajib - Kelas XI*).
  - `body-md` / `body-sm`: Announcements, assignment briefs, and metadata (*Tenggat: 24 Okt 2024*).
  - `label-*`: Button labels, form legends, navigation items, and wireframe annotation tags.

## Layout & Spacing

The layout is grounded in a flexible 4-column (mobile) and 12-column (tablet/desktop) fluid grid system anchored by a baseline 8px module.

- **Page Padding**: Standard mobile canvases enforce an absolute horizontal margin of `16px` (`margin: 1rem`). Outer edges remain uncluttered to accommodate single-hand smartphone usage.
- **Adaptive Breakpoints**:
  - **Mobile (<640px)**: 4 columns, 16px margins, 16px gutters. Stacked single-column layouts for task lists and grades.
  - **Tablet (640px - 1024px)**: 8 columns, 24px margins, 16px gutters. Split-pane layout for schedule overview and assignment submissions.
  - **Desktop (>1024px)**: 12 columns, 32px margins, 24px gutters, max content container width of 1200px.
- **Component Spacing Rhythm**:
  - `space-xs` (4px): Micro-spacing between icon and adjacent text label.
  - `space-sm` (8px): Form field label-to-input gap; vertical separation between subheadings and content.
  - `space-md` (16px): Standard internal card padding; gap between standard interactive elements.
  - `space-lg` (24px): Vertical space between distinct logical sections (*Jadwal Hari Ini* to *Pengumuman Sekolah*).
  - `space-xl` (32px): Deep page separation and bottom action bar offsets.

## Elevation & Depth

To preserve strict low-fidelity wireframe authenticity, elevation shadows, blurs, and pseudo-skeuomorphic depth cues are completely forbidden. Hierarchy is established exclusively via **tonal layering** and **low-contrast outlines**:

- **Level 0 (Canvas Base)**: Pure `#FFFFFF`.
- **Level 1 (Card & Module Containers)**: `#FFFFFF` surface with a crisp `1px solid #E5E7EB` border. Alternatively, `#F3F4F6` surface without borders for secondary grouped sections.
- **Level 2 (Active/Selected Containers & Dialogs)**: `#FFFFFF` fill bounded by a distinct `1.5px solid #111827` stroke.
- **Z-Index Layering (Modal/Bottom Sheet)**: Backdrop overlays use a flat `#111827` tint at 40% opacity. The sheet surface sits flat with a 1px solid stroke separating it from the scrim.

## Shapes

The geometric rule throughout the design system mandates a uniform `8px` (`0.5rem`) corner radius for primary interaction containers:
- Input fields, text areas, standard buttons, and structural cards use `roundedness: 2` (8px).
- Small tags and status chips utilize a half-step `4px` radius to maintain visual proportion against their micro dimensions.
- Box placeholders and image bounds maintain the standard 8px radius to emulate structural containment.
- Pure circular containers are reserved solely for user profile avatar placeholders and icon-only floating action containers.

## Components

### Buttons
- **Touch Ergonomics**: All interactive buttons enforce a strict minimum height of `48px` and horizontal padding of `16px` to meet accessibility criteria.
- **Primary Button**: Solid `#111827` fill, `#FFFFFF` text (`label-lg`), 8px border radius. Hover/active state mapped to `#374151`.
- **Secondary Button**: Transparent `#FFFFFF` fill, 1px solid `#111827` border, `#111827` text.
- **Tertiary/Ghost Button**: Transparent fill, no border, `#374151` text with underline or trailing chevron.
- **Disabled Button**: `#F3F4F6` background, 1px solid `#E5E7EB`, text `#9CA3AF`.

### Input Fields & Controls
- **Text Inputs**: Minimum height of `48px`, `#FFFFFF` background, `1px solid #9CA3AF` border, 8px radius, `12px 16px` padding. Focus state switches border to `2px solid #111827`. Placeholder text rendered in `#9CA3AF` (*Contoh: 12345678*).
- **Labels**: Rendered above the input field in `label-md` using `#111827`, spaced by `8px`.
- **Checkboxes & Radios**: Minimum `20px x 20px` visual box within a `48px x 48px` touch target. Outlined with `1.5px solid #374151`. Checked state renders solid `#111827` with a white checkmark or inner dot.

### Cards & Content Modules
- Surface: `#FFFFFF` with `1px solid #E5E7EB` border and `8px` border radius.
- Padding: `16px` uniform internal spacing.
- Header row cleanly separates the title (`title-md`) from meta actions (*Lihat Semua*) using standard flex alignment.

### Wireframe Placeholders & Media Boxes
- **Box Placeholder (Image / Media)**: Rectangular container filled with `#F3F4F6` and outlined with `1px dashed #9CA3AF`. Crossed diagonal lines ('X') drawn from corner to corner using `1px solid #E5E7EB`. Centered label text reads `[Gambar]` or `[Foto Siswa]` in `label-sm` (`#6B7280`).
- **Logo Placeholder**: Rectangular or square container with `1px solid #9CA3AF`, containing centered text `[Logo Sekolah]` or `[Logo ScholaNexa]`.
- **Avatar Placeholder**: 40px or 48px circular container filled with `#F3F4F6`, outlined with `1px solid #9CA3AF`, containing an outlined person silhouette or initials (`[Foto]`).

### Outline Icons
- Simple single-weight vector outlines drawn at `24px x 24px` with a uniform `1.5px` or `2px` stroke weight in `#111827` or `#6B7280`. No fills, duotone effects, or gradients.

### Chips & Badges
- Height: `28px` to `32px`.
- Status indicators for assignments and presence:
  - *Terkirim* (Submitted): Border `1px solid #111827`, fill `#F3F4F6`, text `#111827`.
  - *Belum Selesai* (Pending): Border `1px dashed #6B7280`, fill `#FFFFFF`, text `#374151`.
  - *Terlambat* (Late): Border `1px solid #374151`, fill `#374151`, text `#FFFFFF`.