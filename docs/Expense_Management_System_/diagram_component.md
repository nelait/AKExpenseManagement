Below is a markdown file containing a Mermaid.js flowchart that represents the component diagram for an Expense Management System. The system components are grouped by layer: Frontend, Backend, Data, and External. I've used subgraphs for layers and arrows to show dependencies between components.

```markdown
# Expense Management System Component Diagram

```mermaid
flowchart TB
    %% Define subgraphs for each layer
    subgraph Frontend
        direction TB
        FE1[User Interface]
        FE2[Expense Reporting Module]
        FE3[Upcoming Expenses Module]
    end

    subgraph Backend
        direction TB
        BE1[Expense Management Service]
        BE2[Report Generation Service]
        BE3[Upcoming Expenses Service]
        BE4[Authentication & Authorization Service]
    end

    subgraph Data
        direction TB
        DB1[(Expense Database)]
        DB2[(User Database)]
    end

    subgraph External
        direction TB
        EXT1[Payment Gateway]
        EXT2[Notification Service]
    end

    %% Define relationships between components
    %% Frontend to Backend
    FE1 --> BE1
    FE2 --> BE2
    FE3 --> BE3

    %% Backend to Data
    BE1 --> DB1
    BE2 --> DB1
    BE3 --> DB1
    BE4 --> DB2

    %% Backend to External
    BE1 --> EXT1
    BE3 --> EXT2

    %% Authentication relationships
    FE1 --> BE4
    FE2 --> BE4
    FE3 --> BE4
```
```

This diagram captures the core components and their interactions within the Expense Management System, aligning with the specified requirements. The Frontend layer contains the user interface and modules for expenses and reporting. The Backend layer handles the core services for managing expenses, generating reports, and managing upcoming expenses, as well as authentication. The Data layer includes databases for expenses and user information. Lastly, the External layer consists of integrations with a payment gateway and a notification service.