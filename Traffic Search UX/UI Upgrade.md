# Traffic Search UX/UI Upgrade Prompt

Act as a Senior Product Designer + Senior Frontend Engineer specializing in map-based search experiences, smart city dashboards, and modern UX systems.

Redesign the current traffic search experience for the Khon Kaen traffic monitoring system.

## Core Objective

Create a premium, modern, highly usable traffic search experience that allows users to search ONLY among the predefined 25 traffic points from `traffic-points.json`.

If the searched keyword is not within those 25 points, the system must gracefully show a professional "Not Found" state.

The UX should feel inspired by:

* Google Maps
* Apple Maps
* Uber
* Grab
* Waze
* Linear command palette

Avoid generic dropdown/select UX.

---

# Data Source

Use:

* `frontend/src/data/traffic-points.json`

This file is the ONLY search source.

Do NOT use:

* external APIs
* Google Places
* global location search

The system must behave as a controlled traffic-location search experience.

---

# UX Requirements

## Search Bar

Design a premium floating search bar:

* rounded corners (18px–24px)
* soft shadow
* subtle border
* modern typography
* left search icon
* right clear/reset button
* smooth focus transition
* mobile-friendly touch size

The search bar must feel modern and production-grade.

---

# Search Experience

Implement:

* search-as-you-type
* fuzzy search
* partial matching
* keyword matching
* keyboard navigation
* smooth dropdown animations

Supported:

* Thai text
* partial Thai keyword search

Examples:

* "มิตร"
  → should match ถนนมิตรภาพ

* "ศรี"
  → should match ถนนศรีจันทร์

---

# Suggestion System

Before typing:

* show suggested traffic points
* show popular locations
* show recent searches

The suggestion panel should feel similar to:

* Google Maps search
* Apple Maps search sheet
* Linear command menu

Use:

* grouped suggestions
* hover state
* active keyboard selection state
* subtle transitions

---

# Result Card UX

Each result should be displayed as a modern card.

Each card should contain:

* traffic icon
* title
* short description
* optional traffic status badge
* hover animation
* clickable interaction

Example hierarchy:

* Primary: route title
* Secondary: route description
* Tertiary: traffic status

---

# Not Found State

If the user searches outside the 25 supported points:

Show a premium empty state.

Example tone:

"ไม่พบเส้นทางนี้"

"ระบบรองรับเฉพาะ 25 จุดจราจรในเมืองขอนแก่น"

Include:

* recommended searches
* suggested traffic points
* helpful UX guidance

Do NOT show harsh error messages.

---

# Map Interaction

When selecting a search result:

* focus the map to that traffic point
* highlight the selected route
* smoothly animate camera movement
* visually emphasize the selected point

---

# Technical Requirements

Frontend stack:

* React or Next.js
* Tailwind CSS
* shadcn/ui
* cmdk or command-menu style architecture
* Fuse.js for fuzzy search

The implementation must be:

* responsive
* accessible
* keyboard navigable
* mobile optimized
* smooth animated
* production quality

---

# Mobile UX

On mobile:

* use bottom sheet style interaction
* expandable search UI
* full-screen search mode if needed
* optimized touch targets
* smooth drag/transition behavior

Inspired by:

* Google Maps mobile search
* Apple Maps mobile interaction

---

# Visual Style

Design language:

* glassmorphism (subtle only)
* modern shadows
* soft gradients
* clean spacing
* premium typography
* dark/light compatible
* minimal but highly polished

Avoid:

* outdated admin dashboard UI
* basic HTML select boxes
* crowded layouts
* harsh colors

---

# Performance Requirements

The search interaction should feel instant.

Optimize:

* filtering
* rendering
* animations
* keyboard interaction

Avoid lag.

---

# Deliverables

Generate:

1. New Search Component
2. Search Dropdown / Suggestion Panel
3. Empty State UI
4. Mobile Responsive Version
5. Search Logic using traffic-points.json
6. Fuse.js integration
7. Keyboard navigation support
8. Modern animations
9. Map focus interaction
10. Clean component architecture

Code quality should reflect senior-level production frontend engineering.
