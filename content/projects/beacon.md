+++
title = "Beacon"
date = 2024-06-20
weight = 2

[taxonomies]
tags = ["flutter", "ar", "accessibility", "mobile-app", "firebase"]

[extra]
github = "https://github.com/Shanu-Kumawat/Beacon"
featured = true
+++

AR-powered navigation app designed specifically for people with visual impairments, featuring real-time object detection and voice-guided pathfinding.

**Accessibility-first design** | Built to serve 285M visually impaired people worldwide

<!-- more -->

## The Challenge

Building a navigation system that could guide users through both indoor and outdoor spaces using voice commands and real-time object detection, all while maintaining smooth performance on mobile devices where processing power is limited.

## Technical Implementation

**Core Framework:** Built with Flutter and Dart for cross-platform mobile deployment. Firebase handles authentication and data storage, while AR Kit provides spatial awareness and environmental understanding.

**Navigation System:** Integrated OpenStreetMap and OpenRouteService to deliver accurate pathfinding that works both indoors and outdoors. The voice interaction uses Flutter's TTS (Text-to-Speech) and Speech-to-Text packages to enable completely hands-free operation.

**Performance Optimization:** The most challenging aspect was balancing accuracy with performance. Object detection needs to happen in real-time to be useful for navigation, but running computer vision models on mobile devices is resource-intensive. I implemented a priority system that focuses processing power on detecting obstacles and navigation-critical objects rather than trying to identify everything in view, keeping the app responsive while maintaining safety.

**Emergency Features:** Designed with real safety concerns in mind. Users can trigger emergency calls or send SMS messages with their current location to predefined contacts—hospitals, police, or family members. This required careful integration with device telephony features and location services, along with building a reliable system that works even when network connectivity is limited.

## Key Features

- **Real-Time Navigation** — Voice-guided pathfinding for indoor and outdoor environments
- **Object Detection** — AR-based detection of obstacles and navigation-critical objects
- **Voice Commands** — Completely hands-free operation via TTS and Speech-to-Text
- **Emergency SOS** — One-tap emergency calling with automatic location sharing
- **Offline Support** — Core navigation works without constant internet connectivity
- **Community Routes** — Users can share helpful navigation paths

## Tech Stack

**Frontend:** Flutter, Dart  
**AR & Spatial:** AR Kit  
**Navigation:** OpenStreetMap, OpenRouteService  
**Backend:** Firebase (Auth, Firestore)  
**Voice:** Flutter TTS, Speech-to-Text  
**ML:** Custom object detection models optimized for mobile

## What I Learned

This project taught me how to design for accessibility, which requires thinking about user interfaces in fundamentally different ways. It showed me the importance of performance optimization in mobile development—when your app guides someone through physical space, lag or failure isn't just annoying, it's potentially dangerous.

I learned how to profile performance, identify bottlenecks, and make architectural decisions that balance functionality with the constraints of mobile hardware. Most importantly, I learned that building for accessibility isn't a feature—it's a fundamental design philosophy that influences every technical decision.

**Impact:**
- Targets 285M visually impaired users globally
- Voice-first interface requires zero visual interaction
- Emergency features designed for life-saving situations
- Battery-optimized to last a full day despite heavy AR/camera usage
