# TASKS.md

# Lohbeng Development Tasks

## Current Sprint Goal

Build a presentation-ready smart city AI dashboard with:

* intelligent traffic monitoring
* pollution analytics
* vehicle tracking visualization
* AI-inspired CCTV monitoring
* futuristic UI/UX

---

# Frontend Tasks

## Dashboard System

### High Priority

* [ ] Build smart metric cards
* [ ] Add animated counters
* [ ] Add PM2.5 visualization
* [ ] Add traffic density indicators
* [ ] Add risk-level badges
* [ ] Add realtime-like polling updates

---

## Smart Map System

### High Priority

* [ ] Integrate MapLibre GL JS
* [ ] Configure OpenStreetMap tiles
* [ ] Add traffic markers
* [ ] Add pollution heatmap
* [ ] Add animated vehicle markers
* [ ] Add CCTV map pins

### Medium Priority

* [ ] Add animated pulses
* [ ] Add floating map analytics
* [ ] Add risk overlays
* [ ] Improve marker clustering

---

## CCTV Monitoring UI

### High Priority

* [ ] Build CCTV preview cards
* [ ] Add fake live-feed animation
* [ ] Add AI tracking overlays
* [ ] Add vehicle detection labels
* [ ] Add animated scan effects

### Medium Priority

* [ ] Add fullscreen mode
* [ ] Add AI detection statistics
* [ ] Add tracking timeline UI

---

## Analytics & Charts

### High Priority

* [ ] Add pollution trend chart
* [ ] Add traffic analytics chart
* [ ] Add vehicle count visualization
* [ ] Add realtime risk indicators

### Medium Priority

* [ ] Add historical simulation charts
* [ ] Add comparative analytics
* [ ] Add district filtering

---

## UI/UX Polish

### High Priority

* [ ] Improve glassmorphism
* [ ] Improve spacing consistency
* [ ] Improve typography hierarchy
* [ ] Improve responsive layout
* [ ] Improve animation smoothness

### Medium Priority

* [ ] Add loading skeletons
* [ ] Add hover interactions
* [ ] Add motion transitions
* [ ] Improve dark mode polish

---

# Backend Tasks

## FastAPI Setup

### High Priority

* [ ] Setup FastAPI server
* [ ] Create modular router structure
* [ ] Configure CORS
* [ ] Create health check endpoint

---

## AI Detection Pipeline

### High Priority

* [ ] Integrate YOLOv8
* [ ] Setup OpenCV pipeline
* [ ] Integrate ByteTrack
* [ ] Implement frame sampling
* [ ] Generate detection JSON exports

### Medium Priority

* [ ] Optimize inference speed
* [ ] Improve tracking stability
* [ ] Add lightweight caching
* [ ] Improve detection filtering

---

## Analytics Engine

### High Priority

* [ ] Build emission score calculator
* [ ] Build pollution risk engine
* [ ] Generate traffic metrics
* [ ] Generate PM2.5 estimation

### Medium Priority

* [ ] Add comparative analytics
* [ ] Add simulation variance logic
* [ ] Add validation metrics

---

# API Tasks

## Required Endpoints

### High Priority

* [ ] GET /api/metrics
* [ ] GET /api/detections
* [ ] GET /api/pollution-risk
* [ ] GET /api/cctv

### Medium Priority

* [ ] GET /api/analytics/history
* [ ] GET /api/map/heatmap

---

# Performance Tasks

### High Priority

* [ ] Optimize frontend rerenders
* [ ] Optimize polling updates
* [ ] Optimize map rendering
* [ ] Reduce animation lag

### Medium Priority

* [ ] Add lazy loading
* [ ] Add dynamic imports
* [ ] Optimize bundle size

---

# Deployment Tasks

## Frontend

* [ ] Configure Vercel deployment
* [ ] Configure environment variables
* [ ] Optimize production build

---

## Backend

* [ ] Configure Railway/Render deployment
* [ ] Configure FastAPI startup
* [ ] Optimize inference runtime

---

# Final Presentation Tasks

### High Priority

* [ ] Prepare smooth demo flow
* [ ] Prepare presentation screenshots
* [ ] Verify responsive layouts
* [ ] Verify stable analytics updates
* [ ] Verify animation quality

---

# Design Approval Workflow

Before major UI redesigns:

* AI MUST propose upgrade plans first
* UI changes require approval
* Stitch AI references remain the source of truth

---

# Engineering Guardrails

## MUST NOT

* introduce Prisma
* introduce Docker
* introduce Redis
* introduce WebSockets
* over-engineer architecture
* redesign the UI completely

---

# Current Priority Order

1. Dashboard UI
2. Smart Map
3. CCTV Interface
4. AI Analytics
5. Motion Polish
6. Backend Optimization

---

# Definition of Done

A task is complete when:

* visually polished
* responsive
* stable during demo
* smooth animations
* no TypeScript errors
* no ESLint issues
* architecture remains consistent
