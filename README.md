# LINE Digital Health Gateway (KPPMCH)

**Integrated Service Orchestration | 8-Grid High-Availability Interface | Nurse-Validated**

An enterprise-grade LINE Official Account (OA) framework designed as the "Digital Front Desk" for Kamphaeng Phet Municipal Community Hospital. This gateway orchestrates multiple clinical services into a single, user-centric mobile interface, ensuring 24/7 healthcare accessibility.

---

## 1. System Architecture & Service Flow

The system acts as a centralized middleware connecting citizens directly to hospital services via a structured rich-menu interface.

### 🔄 Service Orchestration Diagram
```mermaid
graph TD
    %% User Layer
    User[Patient / Citizen] --- LINE[LINE Official Account]

    %% Webhook Event Layer
    LINE --> Webhook{LINE Webhook: Next.js}

    %% Service & Payload Orchestration
    Webhook --> Tele[Telemedicine: Next.js]
    Webhook --> FAQ[FAQ: Flex Payload]
    Webhook --> Roster[Medical Roster]
    Webhook --> News[News Feed API]

    %% Data Layer
    Tele --- DB[(Patient Database)]

    %% Styling
    style Webhook fill:#f9f,stroke:#333,stroke-width:2px
    style LINE fill:#28a745,color:#fff
    style Tele fill:#000,color:#fff
