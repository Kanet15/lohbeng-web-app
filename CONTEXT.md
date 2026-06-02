# CONTEXT.md

# Lohbeng Project Context

## Current Project State

### Project Status

Active Hackathon Development

### Current Phase

Prototype & UI/UX Development Phase

### Development Priorities

1. Build presentation-ready dashboard
2. Complete smart map visualization
3. Integrate AI analytics pipeline
4. Improve smooth UI interactions
5. Create believable smart-city simulation

---

# Current Architecture

```txt id="srk3go"
Frontend (Next.js 16)
        ↓
REST API
        ↓
FastAPI AI Engine
        ↓
YOLO + OpenCV + ByteTrack
        ↓
Analytics Engine
```

---

# Frontend Context

## Frontend Stack

* Next.js 16
* App Router
* TypeScript
* Tailwind CSS v4
* Zustand
* Framer Motion
* shadcn/ui
* MapLibre GL JS

---

## Frontend Responsibilities

The frontend currently handles:

* dashboard rendering
* smart analytics cards
* polling
* map rendering
* CCTV UI
* animation system
* responsive layouts
* data visualization

---

## Frontend Design Direction

The design MUST follow:

* Stitch AI references
* futuristic smart-city UI
* glassmorphism aesthetics
* premium analytics dashboard style

The UI should feel:

* cinematic
* intelligent
* modern
* high-tech
* presentation-ready

---

## Current Frontend Priorities

### High Priority

* Smart dashboard layout
* Animated metrics
* Responsive map system
* CCTV interface
* Pollution visualization

### Medium Priority

* Loading skeletons
* Motion polish
* Transition refinement
* Mobile optimization

---

# Backend Context

## Backend Stack

* FastAPI
* OpenCV
* YOLOv8
* ByteTrack
* NumPy
* Pandas

---

## Backend Responsibilities

The backend currently handles:

* vehicle detection
* object tracking
* analytics calculations
* pollution score generation
* traffic metrics
* JSON export generation

---

## AI Processing Pipeline

```txt id="h2qn0x"
Video Input
    ↓
Frame Sampling
    ↓
YOLO Detection
    ↓
ByteTrack Tracking
    ↓
Analytics Engine
    ↓
Risk Calculation
    ↓
JSON Metrics Export
```

---

# Current Engineering Philosophy

The project intentionally prioritizes:

* fast iteration speed
* visual quality
* believable simulation
* smooth interactions
* modular architecture

The project intentionally avoids:

* enterprise infrastructure
* unnecessary abstractions
* heavy DevOps
* over-engineering

---

# Important Technical Constraints

## MUST USE

* REST APIs
* polling
* modular components
* stateless APIs
* feature-based structure

---

## MUST NOT USE

* Prisma
* PostgreSQL
* Redis
* Docker
* Kubernetes
* WebSockets
* socket.io
* Redux
* microservices

---

# Polling Strategy

Frontend synchronization uses:

* interval polling every 3000ms

Reason:

* simpler architecture
* Vercel compatibility
* hackathon stability
* easier debugging

---

# Data Strategy

The project currently uses:

* mock datasets
* simulated metrics
* generated analytics
* heuristic-based scoring

The project does NOT currently use:

* production databases
* live government APIs
* cloud streaming systems

---

# Analytics Logic

## Pollution Risk Formula

\text{Emission Score}=(\text{Traffic Density}\times0.4)+(\text{Idling Penalty}\times0.4)+(\text{Vehicle Weight Factor}\times0.2)

---

# Current Risk Levels

| Risk      | Color  |
| --------- | ------ |
| Safe      | Green  |
| Moderate  | Yellow |
| Risky     | Orange |
| Dangerous | Red    |

---

# AI Agent Working Rules

AI MUST:

* preserve architecture consistency
* reuse existing components
* keep implementation modular
* maintain design consistency
* follow Stitch AI references

AI SHOULD:

* suggest improvements before implementation
* avoid drastic redesigns
* prioritize UI smoothness
* keep code readable

AI MUST NOT:

* redesign the architecture
* introduce unsupported technologies
* over-engineer systems
* create unnecessary abstractions

---

# UI Upgrade Workflow

Before major UI upgrades:
AI MUST:

1. explain proposed changes
2. explain affected sections
3. explain visual improvements
4. wait for approval first

---

# Current Development Goal

The final hackathon demo should resemble:

* a futuristic AI operations center
* a smart-city command dashboard
* an intelligent urban analytics platform

NOT:

* a generic admin panel
* a CRUD dashboard
* an ERP interface

---

# Final Context Notes

This project is:

* frontend-first
* AI-assisted
* visualization-heavy
* demo-oriented
* presentation-focused

All engineering decisions should support:

* smooth demos
* believable analytics
* polished UI/UX
* rapid development
