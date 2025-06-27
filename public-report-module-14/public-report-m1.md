# Public Report

<br>

<p align="center">
  <img src="../img/inteli-logo.png" alt="Protótipo de baixa fidelidade - tela inicial" width="300">
</p>
<h4 align="center">Giovana Lisbôa Thomé <br> Computer Science <br> Class of 2025 <br> 2025-1B-T02-G56</h4>

<br>

Table of contents:

- [Public Report](#public-report)
- [1. Introduction](#1-introduction)
- [2. Business description](#2-business-description)
- [3. Artifacts](#3-artifacts)
  - [Sprint 1: Project Charter and Project Plan](#sprint-1-project-charter-and-project-plan)
  - [Sprint 2: End-to-End Integration Proof of Concept](#sprint-2-end-to-end-integration-proof-of-concept)
  - [Sprint 3: Dialog Mechanism Implementation and Automated Testing Suite](#sprint-3-dialog-mechanism-implementation-and-automated-testing-suite)
  - [Sprint 4: Dialog and File Analysis Integration](#sprint-4-dialog-and-file-analysis-integration)
  - [Sprint 5: Meta API Integration and Cloud Deployment](#sprint-5-meta-api-integration-and-cloud-deployment)
- [4. Conclusion](#4-conclusion)
- [5. References](#5-references)

# 1. Introduction

This document provides a clear roadmap of the developments carried out during the 1B module of the 2025 academic year, which spanned a duration of 10 weeks.

Students were encouraged to develop final projects aligned with one of three career tracks: academic, corporate, or entrepreneurial. This project followed the entrepreneurial path, which focuses on creating a product or solution with a computing core and building a business around it.

The idea emerged from a relevant context in Brazil, where financial literacy remains low—only 35% of the population demonstrates basic knowledge of financial concepts (OECD, 2020)—and complex financial products often contribute to over-indebtedness. Managing personal finances is also a repetitive and time-consuming task, and traditional financial apps are not always as practical or engaging as a simple message-based interaction. Given the high penetration of messaging platforms like WhatsApp—installed on over 98% of smartphones in the country (DataReportal, 2024)—there is a clear opportunity to deliver accessible and effective financial guidance through a more familiar and user-friendly format.

The module directly built upon the foundational infrastructure of the previously developed AInalytics API. By leveraging that API, the team implemented a fully end-to-end proof of concept that ingests raw transaction data, applies AI-driven analysis, and delivers personalized financial insights through a messaging interface. As a proof of concept, the entire solution was deployed in the cloud, ensuring scalability, reliability, and seamless integration across all service components.

# 2. Business description

The proposed business consists of a personal AI assistant that analyzes individual financial data and communicates insights through a messaging-based interface. The solution aims to deliver clear, concise, and actionable advice on personal finances using natural language, helping users better understand their spending, plan ahead, and improve their financial habits.

By integrating with platforms users already engage with daily, such as WhatsApp, the assistant minimizes friction and meets people where they are. The business leverages conversational AI to offer an intuitive and low-effort alternative to traditional apps, making personal finance management more accessible—especially for users with limited time, financial knowledge, or motivation to engage with complex tools.

# 3. Artifacts

At the beginning of the module, a backlog was created to guide the work over the 10-week period. However, as is often the case, the need for replanning emerged along the way. The following sections outline the discrepancies between the initial plan and the actual deliverables, along with brief descriptions of each artifact produced.

## Sprint 1: Project Charter and Project Plan

The Project Charter and a detailed Project Plan were delivered, defining scope, objectives, timeline, and risks. These documents laid the foundation for governance and progress tracking throughout the ten-week module, ensuring alignment with stakeholder expectations.

## Sprint 2: End-to-End Integration Proof of Concept

An end-to-end proof of concept was delivered, demonstrating the full flow from WhatsApp message capture to the generation of the seusGastos.csv file via the AInalytics API. This artifact validated the transaction-processing architecture and produced actionable data, while identifying future integration points with Meta’s API.

## Sprint 3: Dialog Mechanism Implementation and Automated Testing Suite

A .NET 8 service named MessageManager was delivered, responsible for session management, intent recognition, and simulated responses. Key modules—controllers, session manager, and message service—were structured using dependency injection and singleton patterns, preparing the application for real conversational flows.

A Postman test collection was delivered to automate validation of the MessageManager endpoints. Tests covering session lifecycle, intent recognition, and mock-response behavior were provided, ensuring robustness of the dialogue logic.

## Sprint 4: Dialog and File Analysis Integration

Endpoints for file upload, CSV conversion, and financial analysis via the AInalytics API were delivered and orchestrated asynchronously. This artifact refined the conversational flow to support statement uploads and deliver personalized financial summaries, proving the user experience concept.

## Sprint 5: Meta API Integration and Cloud Deployment

Full integration with Meta’s WhatsApp API was completed, and all services (messaging broker, AInalytics API, MessageManager) were deployed to a cloud environment. This final delivery ensured scalability, high availability, and readiness for real-world use.

# 4. Conclusion

The project achieved its objectives by delivering a minimum viable proof of concept that integrates transaction ingestion, AI-driven analysis, and a conversational interface on WhatsApp. The solution is now operating in testing mode, during which user interactions and performance metrics are being collected to validate the anticipated value gains in financial literacy and user engagement. Future enhancements—such as historical data comparison, interactive graphs, and more advanced financial analysis—will bring additional value and help differentiate this product from conventional personal finance management tools.

# 5. References

DATAREPORTAL. Digital 2024: Brazil. 2024. Disponível em: https://datareportal.com/reports/digital-2024-brazil. Acesso em: 11 abr. 2025.

OECD. OECD/INFE international survey of adult financial literacy. Paris: OECD Publishing, 2020. Disponível em: https://www.oecd.org. Acesso em: 10 abr. 2025.
