# WEB Application Development Prompt

## Application Type: Web Application
## Category: Full-Stack Development
## Template: Modern Web

---

**IMPORTANT**: This is a comprehensive development prompt for building a web application. Follow ALL guidelines, standards, and precautions outlined below for optimal code quality, security, and maintainability.

## Project Description
Expense Management Web application.

## 🎯 Project Overview

**Description**: Expense Management Web application.

**Key Features to Implement**:


**Development Approach**: Follow the guidelines and standards outlined in this prompt to ensure high-quality, maintainable, and secure code.

## 📋 Project Reference Documents

> **Note for AI coding tools**: Read the full documents referenced below for complete context before implementing.

### Technology Stack & Architecture

# Technology Recommendations for Expense Management System

## 1. Frontend Technologies

- **React.js**: A popular JavaScript library for building user interfaces, React.js offers component-based architecture, which enhances reusability and scalability. It is widely supported and has a large community, making it a practical choice for building dynamic and responsive UI.

...

📄 **Full document**: @docs/techstack.md

---

### Backend Implementation Guide

```markdown
# Expense Management System Backend Implementation Guide

**Version:** 1.0  
**Date:** 2/20/2026

---

## 1. API Design

### Key Endpoints

#### Expenses Management
- **GET /api/expenses**  
  - **Description:** Retrieve all expenses.
  - **Response Payload:**  
    ```json
    [
      {
        "id": "string",
        "amount": "number",
        "category": "string",
        "date": "date",
        "description": "string"
      }
    ]
    ```

- **POST /api/expenses**  
...

📄 **Full document**: @docs/backend.md

---

### Project Status & Progress

# Project Status Tracking Template: Expense Management System

---

## 1. Implementation Phases

### Phase 1: Expense Management Module
- **Goal**: Develop the core functionality to manage expenses.
- **Tasks**:
  - Design database schema for expense tracking.
  - Implement expense entry features.
  - Develop functionality for categorizing expenses.
  - Create user interface for managing expenses.

### Phase 2: Reporting Capabilities
...

📄 **Full document**: @docs/status.md

---

### diagram_component

Below is a markdown file containing a Mermaid.js flowchart that represents the component diagram for an Expense Management System. The system components are grouped by layer: Frontend, Backend, Data, and External. I've used subgraphs for layers and arrows to show dependencies between components.

```markdown
# Expense Management System Component Diagram

```mermaid
flowchart TB
    %% Define subgraphs for each layer
    subgraph Frontend
        direction TB
        FE1[User Interface]
...

📄 **Full document**: @docs/diagram_component.md

---

### diagram_architecture

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

...

📄 **Full document**: @docs/diagram_architecture.md

---

### Requirements Specification

# Expense Management System Requirements Document

## 1. Project Overview

The project entails the development of an Expense Management System designed to efficiently handle and track expenses. The system aims to provide users with the ability to manage their current expenses, prepare for upcoming expenses, and generate comprehensive reports on financial activities. This system will serve as a tool for both personal and professional financial management, ensuring users can maintain clear insight
...

📄 **Full document**: @docs/requirements.md

---

### Frontend Implementation Guide

# Frontend Implementation Guide for Expense Management System

This guide provides a detailed plan and code examples for implementing the frontend of an Expense Management System. The system includes features for managing expenses, generating reports, and handling upcoming expenses.

## 1. Component Structure

### Main Components
- **ExpenseDashboard**: Displays an overview of current expenses, upcoming expenses, and recent activity.
...

📄 **Full document**: @docs/frontend.md

---

### Application Flow & User Journeys

# Expense Management System Flow Documentation

## 1. User Workflows

### Overview
Users will interact with the Expense Management System through a web or mobile application to manage their expenses, generate reports, and plan for upcoming expenses.

### User Workflows

#### 1.1. Manage Expenses
- **Step 1:** User logs into the system.
- **Step 2:** User navigates to the "Manage Expenses" section.
- **Step 3:** User can add a new expense, view, edit, or delete existing expenses.
...

📄 **Full document**: @docs/flow.md

---

### estimation

Creating a complete project estimation report using Function Point Analysis (FPA) requires a detailed understanding of the project requirements. Below is a fictional, but realistic estimation document for an Expense Management System, filling in the placeholders with hypothetical values based on typical project assumptions.

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
...

📄 **Full document**: @docs/estimation.md

---

### diagram_sequence

Below is a markdown file with Mermaid.js sequence diagrams that illustrate key user flows for an Expense Management System, including authentication, managing expenses, generating reports, and handling upcoming expenses.

```markdown
# Expense Management System Sequence Diagrams

## 1. User Authentication Flow

```mermaid
sequenceDiagram
    actor User
    participant AuthService as Authentication Service
    participant DB as Database

    User ->> AuthService: Enter credentials
...

📄 **Full document**: @docs/diagram_sequence.md

---

### Product Requirements Document (PRD)

# Product Requirements Document (PRD)

## 1. Introduction

The Expense Management System is designed to streamline the management of expenses for individuals and organizations. This system aims to provide users with the ability to manage their expenses efficiently, generate comprehensive reports for better financial insights, and plan for upcoming expenses. This PRD outlines the detailed product specifications, user experience, and implementation requirements necessary to build this system.

...

📄 **Full document**: @docs/prd.md

## 🏗️ Architecture Guidelines

**Pattern**:
- Full-stack monorepo or separate repos, API-first design approach, Shared type definitions, Microservices or monolithic architecture

**Description**:
- Application architecture pattern

**Structure**:
- **directories**: Full-stack monorepo or separate repos, API-first design approach, Shared type definitions, Microservices or monolithic architecture
- **files**: Client-server communication patterns, Database to API to frontend flow, Real-time updates (WebSockets, SSE), Caching strategies across layers
- **conventions**: File-based routing (Next.js style), API route organization, Protected routes and middleware, SEO-friendly routing

**Data Flow**:
- Client-server communication patterns, Database to API to frontend flow, Real-time updates (WebSockets, SSE), Caching strategies across layers

**State Management**:
- React State

**API Design**:
- RESTful

## 📋 Development Guidelines



## 📏 Coding Standards



## 📚 Required Libraries and Dependencies



## 🔒 Security Considerations



## ⚡ Performance Guidelines



## ✨ Best Practices

## 🧪 Testing Guidelines
  
  

## 🚀 Deployment Guidelines
  
  

## ⚠️ Critical Precautions



## 🛠️ Implementation Instructions

Build a responsive web application with modern frontend framework. Ensure cross-browser compatibility and accessibility.

### Development Workflow
1. **Setup**: Initialize project with proper structure and dependencies
2. **Core Implementation**: Build core functionality following architecture guidelines
3. **Security**: Implement security measures as outlined above
4. **Testing**: Write comprehensive tests for all components
5. **Performance**: Optimize based on performance guidelines
6. **Documentation**: Document all APIs, components, and deployment procedures
7. **Deployment**: Follow deployment guidelines for chosen platform

### Quality Checklist
- [ ] All security requirements implemented
- [ ] Performance optimizations applied
- [ ] Comprehensive test coverage achieved
- [ ] Code follows all coding standards
- [ ] Documentation is complete and accurate
- [ ] Deployment configuration is ready

---

## 📚 Final Notes

**Remember**: This prompt contains comprehensive guidelines for building a high-quality application. Prioritize security, performance, and maintainability throughout the development process.

**Code Quality**: Follow all coding standards and best practices outlined above.
**Security First**: Never compromise on security requirements.
**Performance**: Optimize early and measure continuously.
**Testing**: Maintain high test coverage and quality.

**Good luck with your development!** 🚀