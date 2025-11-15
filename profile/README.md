# MicroCODE Regatta RC

**Web and Mobile Application for Regatta Race Committee Scoring**

Regatta RC™ comprehensive regatta management system designed specifically for Race Committee operations, built on the MicroCODE version of the Gravity Zero App platform.

## Overview

Regatta RC™ is a modern web and mobile application that empowers Race Committees to efficiently manage and score sailing regattas in real-time. From single races to multi-day series, Regatta RC provides the tools needed to run professional sailing events.

## Core Entities

The application manages the complete regatta ecosystem:

### Event Management

- **Series**: Collections of regattas occurring on non-contiguous days
- **Regatta**: Collections of races occurring on contiguous days
- **Race**: Individual races between boats with real-time scoring

### Participant Management

- **Boat**: Physical vessels with manufacturing details and certifications
- **Design**: Boat blueprints and specifications for class racing
- **Cert**: Handicapping certificates for boats (PHRF, IRC, etc.)
- **Sail**: Sail inventory and specifications for boats
- **Person**: Sailors, owners, and race officials
- **User**: System users with role-based access control

### Organization Management

- **Region**: Geographic areas organizing sailing activities
- **Org**: Sanctioning bodies and sailing associations
- **Club**: Sailing organizations managing boats and members
- **Prize**: Awards, trophies, and tokens for race winners

### System Infrastructure

- **Config**: Application configuration and product testing
- **App**: Admin tools for cache, Redis, database, and JSON management
- **Support**: Integrated help desk and ticket system

## Architecture

Built on the **MERN** (MongoDB, Express, React, Node.js) stack with a layered API architecture:

## Technology Stack

- **Frontend**: React (Web), React Native (Mobile)
- **Backend**: Node.js with Express
- **UI Framework**: HTMX + HTML/CSS (Hypermedia-driven), Shadcn components
- **Database**: MongoDB (NoSQL)
- **API**: RESTful with both JSDoc and Swagger documentation
- **Authentication**: Multi-level role-based access control
- **Real-Time**: Redis for caching and pub/sub

## Key Features

### Race Committee Tools

- Real-time race scoring and results
- Multi-race regatta management
- Series scoring with various handicapping systems
- Protest and penalty tracking
- Weather and timing integration

### Participant Features

- Boat registration and certification management
- Crew and sail inventory
- Race entry and payment processing (thru STRIPE)
- Results viewing and notifications

### Administrative Tools

- User management with privilege levels (Admin, Chairman, Official, Scorer, Owner, Crew)
- Database and cache management
- System health monitoring
- Support ticket system
- Comprehensive audit logs

### Mobile Support

- Native iOS and Android apps
- Offline capability for race scoring
- Real-time synchronization
- Push notifications

## Role-Based Access

Seven privilege levels ensure appropriate access:

- **Admin**: Full system access
- **Chairman**: Regatta oversight and management
- **Official**: Race officiating and rule enforcement
- **Scorer**: Race scoring and results entry
- **Owner**: Boat and personal data management
- **Crew**: Boat crew members and support staff

## Built With MicroCODE Web App

Regatta RC is built on **MicroCODE Web App**, our internal SaaS development platform derived from the licensed [Gravity SaaS Boilerplate](https://usegravity.app/) by Gravity Zero Ltd.

This provides:

- ✅ Production-ready authentication and authorization
- ✅ Stripe payment integration for race entry fees
- ✅ Multi-tenant architecture for clubs and organizations
- ✅ Responsive UI components with dark mode
- ✅ Email notifications and transactional templates
- ✅ Admin dashboard and analytics
- ✅ API infrastructure with throttling and security
- ✅ Mobile app foundation with React Native

## Development

### API Documentation

All endpoints are automatically documented via Swagger, generated from the single source of truth configuration in `__config.js`.

### Hypermedia Approach

Following principles from "Hypermedia Systems" by Carson Gross et al., the UI leverages HTMX for dynamic, server-rendered content without heavy JavaScript frameworks.

### Dynamic Entity System

Entities are defined once in `__config.js` and automatically generate:

- Database tables and enums
- API endpoints (CRUD operations)
- Swagger documentation
- UI views and forms
- Authorization rules

## Repository Structure

This GitHub Organization contains:

- **regatta-rc-backend**: Node.js API server
- **regatta-rc-frontend**: React web application
- **regatta-rc-mobile**: React Native iOS/Android apps
- **regatta-rc-docs**: Documentation and guides
- **regatta-rc-infra**: Deployment and infrastructure code

## License

© 2022-2025 MicroCODE, Inc. All rights reserved.

This software and related materials are proprietary to MicroCODE, Inc. and contain confidential information. Not for public distribution.

## Contact

**MicroCODE, Inc.**
55 E. Long Lake Rd #224
Troy, MI 48085

📞 +1 855.421.1010
📧 company@mcode.com
🌐 [www.mcode.com](https://www.mcode.com)

---

_Empowering Race Committees with modern technology for professional regatta management._
