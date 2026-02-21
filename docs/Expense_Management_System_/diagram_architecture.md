```markdown
```mermaid
flowchart TB
  %% Define Subgraphs for Layer Separation
  subgraph Presentation Layer
    UI[Web & Mobile UI]
  end

  subgraph Business Logic Layer
    BE[Backend Service]
  end

  subgraph Data Layer
    DB[(Database)]
    Cache[(In-Memory Cache)]
  end

  subgraph Integration Layer
    PaymentGateway[Payment Gateway]
    NotificationService[Notification Service]
  end

  subgraph Reporting Layer
    ReportService[Report Generation Service]
  end

  %% Presentation Layer Connections
  UI --> BE

  %% Business Logic Layer Connections
  BE -->|Read/Write| DB
  BE -->|Cache Management| Cache
  BE -->|Process Payments| PaymentGateway
  BE -->|Send Notifications| NotificationService
  BE -->|Generate Reports| ReportService

  %% Data Layer Connections
  Cache -->|Data Backup| DB

  %% Reporting Layer Connections
  ReportService --> DB

  %% Technology Choices
  UI:::tech -->|React Native| 
  BE:::tech -->|Node.js| 
  DB:::tech -->|PostgreSQL| 
  Cache:::tech -->|Redis| 
  PaymentGateway:::tech -->|Stripe API| 
  NotificationService:::tech -->|Twilio API| 
  ReportService:::tech -->|Python| 

  %% Style Definitions
  classDef tech fill:#f9f,stroke:#333,stroke-width:2px;
```
```
This architecture diagram represents a high-level overview of an Expense Management System, focusing on the separation of concerns across different layers including the Presentation, Business Logic, Data, Integration, and Reporting Layers. Each component is associated with a specific technology choice, and the connections between components illustrate the flow of data and interactions within the system.