![Wellnest Wellness App](assets/cover.svg)

# Wellnest

> A cross-platform wellness companion for nutrition, fitness, hydration, consultations, and food ordering.

[![Case study](https://img.shields.io/badge/case%20study-public%20portfolio-15803D)](SECURITY.md)
[![React Native](https://img.shields.io/badge/React%20Native-0.76-61DAFB?logo=react&logoColor=111827)](https://reactnative.dev/)
[![Redux Toolkit](https://img.shields.io/badge/state-Redux%20Toolkit-764ABC?logo=redux&logoColor=white)](https://redux-toolkit.js.org/)
[![Android + iOS](https://img.shields.io/badge/platform-Android%20%2B%20iOS-111827)](https://reactnative.dev/)

## Overview

Wellnest brings daily wellness actions into one mobile experience. Users complete onboarding and health goals, track meals and hydration, review calorie and macro information, follow workouts, manage target weight, search dietitians, book online consultations, and order food. Separate dietitian and food-provider workspaces support the operational side of the product.

## My contribution

- React Native navigation architecture with auth, onboarding, bottom tabs, and role-specific stacks
- Login, registration, OTP verification, Google sign-in, profile setup, fitness goals, BMI, and target weight journeys
- Food diary, meal records, calorie/macronutrient inputs, meal-type workflows, and image uploads
- Hydration tracking, workout/video screens, progress states, and date/calendar interactions
- Dietitian discovery, online consultation booking, appointment views, and practitioner meal management
- Food-provider catalog, product detail, cart, “for myself / for someone” ordering, and confirmation flows
- API integration, AsyncStorage persistence, Redux Toolkit state, charts, pickers, permissions, and media handling

## Skills demonstrated

| Area | Applied |
| --- | --- |
| Mobile engineering | React Native screens, native stack/bottom tabs, safe areas, reusable controls |
| Wellness UX | Goals, BMI, weight, meals, hydration, workouts, progress, and daily habits |
| Marketplace flows | Dietitian search, consultation booking, food catalog, cart, and order confirmation |
| Role-based product | User, dietitian, and food-provider experiences with dedicated workflows |
| State and data | Redux Toolkit, AsyncStorage, API requests, upload payloads, and local session state |
| Device integration | Google sign-in, date/time pickers, camera/gallery selection, health/fitness bridges, and permissions |

## Wellness operating flow

Wellnest turns onboarding data into a repeatable daily loop: define a goal, complete small wellness actions, review progress, and reach the right practitioner or food provider when support is needed.

```mermaid
flowchart TB
    Welcome[Welcome] --> Auth[Register / sign in]
    Auth --> Verify[Verify account]
    Verify --> Profile[Set profile, goals, and target weight]
    Profile --> Dashboard[Open daily dashboard]

    subgraph HABITS[01 - Build daily habits]
        Meals[Log meals and macros]
        Water[Track hydration]
        Workout[Follow workout]
        Meals --> Progress[Review progress]
        Water --> Progress
        Workout --> Progress
    end

    subgraph CARE[02 - Reach care]
        Search[Find dietitian] --> Slot[Choose consultation slot]
        Slot --> Appointment[Confirm appointment]
    end

    subgraph ORDER[03 - Complete an order]
        Provider[Browse food provider] --> Cart[Build cart]
        Cart --> Order[Place food order]
        Order --> Receipt[Order confirmation]
    end

    Dashboard --> Meals
    Dashboard --> Water
    Dashboard --> Workout
    Dashboard --> Search
    Dashboard --> Provider
    Progress -. return to dashboard .-> Dashboard
```

**Outcome:** a measurable wellness routine with connected practitioner and food-service workflows.

## Technical stack

React Native 0.76 · React Navigation 7 · Redux Toolkit · AsyncStorage · Axios · React Native Paper · Gifted Charts · Calendars · Google Sign-In · Native permissions and media modules.

See [architecture](docs/ARCHITECTURE.md), [user flows](docs/USER-FLOWS.md), [security policy](SECURITY.md), [screenshot guide](docs/SCREENSHOT-GUIDE.md), and [GitHub setup](docs/GITHUB-SETUP.md).
"# wellnest" 
