# EXERCICE

We have to define terms/concepts that relevant for API integration

API Integration Terms & Concepts for Insurance Enterprise Architecture
Given your context (Insurance company, Mulesoft API, Salesforce, recent acquisition), here are the key terms and concepts to define:
Integration Architecture Terms
API (Application Programming Interface)
A set of protocols and tools that allows different software applications to communicate with each other. In your context, APIs will connect Salesforce with legacy insurance systems and the new parent group's platforms.
Mulesoft Anypoint Platform
The integration platform you'll use to connect applications, data, and devices. It provides API design, deployment, management, and analytics capabilities.
API-Led Connectivity
Mulesoft's architectural approach organizing APIs into three layers:

Experience APIs: Tailored to specific channels (mobile, web, partner portals)
Process APIs: Orchestrate business processes (policy underwriting, claims processing)
System APIs: Connect to underlying systems (policy admin, billing, document management)

ESB (Enterprise Service Bus)
Mulesoft's integration framework that routes and transforms messages between applications.
iPaaS (Integration Platform as a Service)
Cloud-based platform (like Mulesoft) for integrating applications across cloud and on-premises environments.
Salesforce-Specific Terms
Salesforce Financial Services Cloud
Industry-specific CRM likely relevant for your insurance operations, managing customer relationships, policies, and household views.
Salesforce Platform Events
Real-time event-driven messaging used to integrate Salesforce with external systems asynchronously.
External Objects
Salesforce feature allowing real-time access to data stored outside Salesforce (like policy data in legacy systems) without data replication.
Connected Apps
OAuth-enabled applications that integrate with Salesforce using standard APIs.
Data Integration Concepts
Master Data Management (MDM)
Critical post-acquisition: establishing single sources of truth for customers, policies, agents, and products across merged entities.
Data Synchronization
Keeping customer, policy, and claim data consistent between Salesforce, Mulesoft, legacy systems, and parent group systems.
Canonical Data Model
Standardized data format within Mulesoft that simplifies transformations between different system formats.
ETL (Extract, Transform, Load)
Process for moving and transforming data between systems, often batch-oriented for historical data migration.
Security & Governance Terms
OAuth 2.0
Industry-standard authorization protocol for secure API access between your systems and the parent group.
API Gateway
Mulesoft component managing API traffic, security policies, rate limiting, and monitoring.
Single Sign-On (SSO)
Enabling users to access multiple systems (Salesforce, parent group portals) with one set of credentials.
API Policies
Security and operational rules applied to APIs (rate limiting, encryption, access control).
Data Residency
Where customer data is stored and processed—critical for insurance regulatory compliance post-acquisition.
Post-Acquisition Specific Terms
System of Record (SOR)
Authoritative source for specific data types. Post-acquisition, you must clarify: Which system owns policy data? Customer data? Financial data?
Legacy System Modernization
Strategy for updating or replacing older insurance systems while maintaining business continuity.
Integration Hub
Centralized architecture pattern where Mulesoft acts as the integration layer between all systems.
B2B Integration
Connecting with external partners (reinsurers, distributors, brokers) and now your parent group's systems.
Insurance-Specific Integration Concepts
Policy Administration System (PAS) Integration
Connecting core insurance policy systems to Salesforce for 360-degree customer view.
Claims Management System Integration
Real-time claims data flowing to Salesforce for agent/customer access.
Rating Engine Integration
Connecting pricing/underwriting systems to provide quotes through Salesforce.
ACORD Standards
Insurance industry data standards that may be used in API payloads for interoperability.
Performance & Monitoring
API Latency
Response time critical for customer-facing operations (quote generation, policy lookups).
Rate Limiting
Controlling API call volumes to prevent system overload.
API Analytics
Monitoring API usage, performance, and errors through Mulesoft Anypoint Monitoring.
Circuit Breaker Pattern
Fault tolerance mechanism preventing cascade failures when systems are unavailable.
