# SPEC.md

# Lohbeng — Intelligent Traffic & Pollution Intelligence Platform

## Project Overview

### Project Name

Lohbeng

### Project Type

Smart City AI Monitoring Platform

### Development Stage

Hackathon Prototype / Presentation Demo

### Primary Goal

Build a futuristic smart-city dashboard capable of:

* vehicle detection visualization
* traffic analytics
* PM2.5 pollution risk monitoring
* CCTV intelligence simulation
* interactive geospatial monitoring
* AI-inspired urban analytics

The project should prioritize:

* smooth UI/UX
* visual quality
* believable AI simulation
* presentation readiness
* fast iteration speed

---

# Core Technology Stack

## Frontend

* Next.js 16 (App Router)
* TypeScript
* Tailwind CSS v4
* Zustand
* shadcn/ui
* Framer Motion
* MapLibre GL JS
* OpenStreetMap

## Backend

* FastAPI
* Python 3.11+
* OpenCV
* YOLOv8
* ByteTrack
* NumPy
* Pandas

---

# Architecture Philosophy

This project uses a lightweight hybrid architecture:

```txt id="ozz11q"
Frontend (Next.js)
        ↓
REST API
        ↓
FastAPI AI Engine
        ↓
YOLO + OpenCV + Tracking
        ↓
Analytics Engine
```

The architecture is intentionally:

* lightweight
* stateless
* modular
* hackathon-friendly
* demo-oriented

Avoid enterprise-scale complexity.

---

# Absolute Engineering Rules

## MUST USE

* TypeScript
* Tailwind CSS v4
* Zustand
* Route Handlers
* REST APIs
* Feature-based architecture
* Modular components

---

## MUST NOT USE

* Prisma
* PostgreSQL
* Redis
* Docker
* Kubernetes
* Socket.io
* WebSockets
* Redux
* Microservices
* Monolithic backend architecture

---

# Frontend Responsibilities

The frontend MUST handle:

* dashboard rendering
* charts
* smart analytics visualization
* polling
* interactive maps
* CCTV UI
* animations
* presentation logic

The frontend MUST NOT:

* perform heavy AI inference
* process video frames
* run OpenCV pipelines
* execute YOLO inference

---

# Backend Responsibilities

The backend MUST handle:

* YOLO inference
* OpenCV frame processing
* ByteTrack tracking
* analytics generation
* pollution score calculations
* vehicle counting
* JSON export generation

The backend MUST remain:

* stateless
* modular
* lightweight

---

# Folder Structure

```txt id="h9s9g7"
/
├── frontend/
│   ├── src/
│   ├── public/
│   └── package.json
│
├── backend/
│   ├── app/
│   │   ├── routers/
│   │   ├── services/
│   │   ├── models/
│   │   ├── utils/
│   │   └── main.py
│   │
│   ├── videos/
│   ├── outputs/
│   ├── weights/
│   └── requirements.txt
│
├── SPEC.md
├── CONTEXT.md
├── TASKS.md
├── DESIGN_RULES.md
└── BEST_PRACTICES.md
```

---

# Core Features

## Smart Traffic Dashboard

Display:

* PM2.5 metrics
* traffic density
* vehicle count
* AI risk levels
* prediction analytics

---

## Interactive Map System

Features:

* live markers
* traffic heatmaps
* pollution zones
* CCTV pins
* animated vehicle tracking

Technology:

* MapLibre GL JS
* OpenStreetMap

---

## CCTV Monitoring System

Features:

* AI-style surveillance UI
* tracking overlays
* animated feed cards
* smart detection simulation

---

## Vehicle Tracking System

Features:

* simulated or real tracking
* live coordinate updates
* object tracking IDs
* traffic movement analytics

---

## AI Analytics Engine

Responsibilities:

* pollution risk scoring
* traffic analysis
* emission calculations
* congestion evaluation

---

# Data Contract

All traffic records MUST follow:

```json id="9zq4zd"
{
  "id": 1,
  "title": "ถ.กัลปพฤกษ์",
  "description": "หน้าตลาดคอมเพล็กซ์",
  "province": "ขอนแก่น",
  "lat": 16.4321,
  "lng": 102.8231,
  "pm25": 75.1,
  "trafficLevel": "high",
  "riskLevel": "danger",
  "vehicles": 124
}
```

---

# Analytics Formula

The emission score MUST follow:

\text{Emission Score}=(\text{Traffic Density}\times0.4)+(\text{Idling Penalty}\times0.4)+(\text{Vehicle Weight Factor}\times0.2)

---

# Risk Thresholds

| Score  | Risk      | Color  |
| ------ | --------- | ------ |
| 0–35   | Safe      | Green  |
| 36–65  | Moderate  | Yellow |
| 66–85  | Risky     | Orange |
| 86–100 | Dangerous | Red    |

---

# API Architecture

## Frontend Communication Strategy

Use:

* REST APIs
* polling every 3000ms

DO NOT use:

* WebSocket
* socket.io

---

# API Endpoints

## GET /api/metrics

Returns:

* PM2.5
* traffic analytics
* vehicle counts
* risk scores

---

## GET /api/detections

Returns:

* YOLO detections
* tracking IDs
* confidence scores

---

## GET /api/pollution-risk

Returns:

* risk analytics
* pollution severity
* emission scores

---

# UI/UX Philosophy

The interface should feel:

* futuristic
* cinematic
* intelligent
* premium
* presentation-ready

The UI MUST follow:

* Stitch AI design references
* glassmorphism aesthetics
* smooth transitions
* floating analytics cards

---

# Design Rules

AI MAY:

* improve spacing
* improve animations
* improve responsiveness
* improve visual hierarchy
* improve typography

AI MUST NOT:

* redesign the entire layout
* ignore Stitch AI references
* change the design language drastically

All major UI upgrades require approval first.

---

# Performance Rules

## Frontend

Prefer:

* lazy loading
* dynamic imports
* localized rerenders
* modular components

---

## Backend

Prefer:

* frame sampling
* lightweight inference
* optimized analytics
* summarized JSON outputs

Avoid:

* unnecessary heavy processing

---

# AI Agent Instructions

AI MUST:

* preserve architecture consistency
* reuse existing components
* avoid over-engineering
* keep implementation modular
* prioritize readability

AI MUST NOT:

* introduce enterprise infrastructure
* create unnecessary abstractions
* add unsupported technologies

---

# Definition of Done

A feature is complete when:

* responsive on desktop & mobile
* no TypeScript errors
* no ESLint issues
* smooth animations
* visually polished
* presentation-ready
* stable during demo
* works correctly on Vercel frontend deployment

---

# Final Philosophy

Lohbeng should feel like:

* a futuristic AI operations center
* a modern urban intelligence platform
* a believable smart city monitoring system

NOT:

* a generic admin dashboard
* a CRUD template
* an enterprise ERP interface
