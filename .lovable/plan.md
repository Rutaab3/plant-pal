

# 🌿 Leafy — Plant Care Journal

A premium botanical-themed plant care journal app with localStorage persistence, beautiful UI, and thoughtful micro-interactions.

---

## Phase 1: Foundation & Design System

- Set up custom color theme (cream base #FAFAF7, sage green #7A9E7E, terracotta #C17D5A, forest text #2D3B2D) with dark mode support
- Add Google Fonts (Playfair Display + Inter)
- Build localStorage hooks (`usePlants`) for CRUD operations with optimistic updates
- Create responsive layout shell: sidebar nav on desktop, bottom tab bar on mobile
- Add botanical SVG decorations and placeholder illustrations

## Phase 2: Dashboard (Home)

- "Leafy" header with leaf logo SVG
- Stats bar: Total Plants, Needs Water Today, Overdue, RIP Archive count
- Overdue Care alert banner with clickable plant links
- Today's Care section with plant cards needing attention
- Floating "+" action button to quick-add plants

## Phase 3: Add/Edit Plant Modal

- Full-screen on mobile, centered modal on desktop
- All fields: name, species, photo URL (with live preview), location dropdown, soil type dropdown, purchase date picker, watering/fertilizing frequency, health status radio pills, notes
- Photo URL fallback to botanical placeholder with plant initial
- Form validation with react-hook-form + zod

## Phase 4: My Garden (Collection Gallery)

- 3-column responsive card grid showing photo, name, species, location badge, health emoji (🟢🟡🔴), watering countdown
- Filter bar: location dropdown, health status, search by name/species
- Sort options: A-Z, Recently Added, Needs Water First
- Illustrated empty state with CTA

## Phase 5: Plant Detail Page

- Hero section with large photo, plant info, "owned X days" counter
- Health status pill selector (instant update)
- Care action buttons row (Water, Fertilize, Repot, Add Note) — each opens mini modal with date picker + optional note
- Care Schedule card with circular progress ring showing days until next watering
- Care Log timeline (chronological, deletable entries)
- Growth Photo Timeline grid with add photo modal
- Danger zone: Mark as RIP, Delete Permanently with confirmation

## Phase 6: Watering Schedule Grid

- 3-week calendar grid (Mon–Sun columns)
- Plant chips colored by health status on their due days
- Past days show ✅ completed or ❌ missed
- Toggle between watering-only and all-care view
- Clickable chips navigate to plant detail

## Phase 7: RIP Archive

- Grayscale card grid of archived plants
- Epitaph style: "Here rests [Name] 🌱 — loved and cared for"
- Restore and Delete Forever buttons per card

## Phase 8: Bonus Features

- Seasonal Care Tips panel detecting current season with relevant tips and "which of my plants" tags
- Dark mode toggle persisted in localStorage
- Export Garden as JSON backup file download
- Import Garden from uploaded JSON file
- Toast notifications for all actions
- Smooth fade/slide transitions on cards and modals
- Health status auto-suggestion toasts when plants are 3+ days overdue

