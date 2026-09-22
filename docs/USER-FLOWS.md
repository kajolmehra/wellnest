# User flows

```mermaid
flowchart LR
    Welcome[Welcome] --> Auth[Register / sign in]
    Auth --> Setup[Profile and goals]
    Setup --> Dashboard[Daily dashboard]
    Dashboard --> Meals[Log meals]
    Dashboard --> Water[Track hydration]
    Dashboard --> Workouts[Open workout]
    Dashboard --> Dietitian[Search and book dietitian]
    Dashboard --> Shop[Order food]
    Shop --> Confirmation[Order confirmation]
```

## Practitioner flow

Dietitians can review appointments, maintain food items, add nutrition values, and review food history. Food providers maintain their business profile and product data so the customer experience stays connected to the operational workflow.
