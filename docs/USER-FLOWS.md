# User flows

```mermaid
flowchart TB
    Welcome[Welcome] --> Auth[Register / sign in]
    Auth --> Verify[OTP / provider verification]
    Verify --> Setup[Profile, goals, BMI, target weight]
    Setup --> Dashboard[Daily dashboard]
    Dashboard --> Meals[Log meal and nutrition]
    Dashboard --> Water[Track hydration]
    Dashboard --> Workouts[Open workout / video]
    Dashboard --> Dietitian[Search dietitian]
    Dietitian --> Appointment[Book consultation]
    Dashboard --> Shop[Browse food provider]
    Shop --> Cart[Build cart]
    Cart --> Confirmation[Order confirmation]
    Meals --> Progress[Review daily progress]
    Water --> Progress
    Workouts --> Progress
    Progress -. continue routine .-> Dashboard
```

## Practitioner flow

Dietitians can review appointments, maintain food items, add nutrition values, and review food history. Food providers maintain their business profile and product data so the customer experience stays connected to the operational workflow. The result is one loop from personal tracking to professional support and fulfillment.
