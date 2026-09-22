# Architecture

Wellnest is a React Native application with a navigation shell that separates onboarding/auth, user wellness, dietitian operations, and food-provider operations. Shared API helpers and Redux state connect screens to the remote JSON API while AsyncStorage preserves local session and lightweight app state.

## Product boundaries

- **Onboarding:** registration, OTP, sign-in, profile, goals, BMI, and target weight.
- **Daily wellness:** meals, food diary, hydration, workouts, progress, and media.
- **Care network:** dietitian search, provider profiles, consultation booking, appointments, and meal plans.
- **Food ordering:** provider catalog, product detail, cart, recipient choice, and confirmation.
- **Platform services:** API requests, local persistence, permissions, image selection, charts, calendars, and role-aware navigation.
