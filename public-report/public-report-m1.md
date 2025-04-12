# Public Report
<br>

<p align="center">
  <img src="img/inteli-logo.png" alt="Protótipo de baixa fidelidade - tela inicial" width="300">
</p>
<h4 align="center">Giovana Lisbôa Thomé <br> Computer Science <br> Class of 2025 <br> 2025-1A-T02-G56</h4>

<br>

Table of contents:
- [Public Report](#public-report)
  - [1. Introduction](#1-introduction)
  - [2. Business description](#2-business-description)
  - [3. Artifacts](#3-artifacts)
    - [3.2. Developed artifacts](#32-developed-artifacts)
      - [3.2.1. TAPI and Project Plan](#321-tapi-and-project-plan)
      - [3.2.2. Application Architecture](#322-application-architecture)
      - [3.2.3. Low Fidelity Prototype](#323-low-fidelity-prototype)
      - [3.2.4. AInalytics API](#324-ainalytics-api)
      - [3.2.5. Product Development Plan and Product Benchmarking](#325-product-development-plan-and-product-benchmarking)
  - [4. Conclusion](#4-conclusion)
  - [5. References](#5-references)

## 1. Introduction

This document provides a clear roadmap of the developments carried out during the 1A module of the 2025 academic year, which spanned a duration of 10 weeks.

Students were encouraged to develop final projects aligned with one of three career tracks: academic, corporate, or entrepreneurial. This project followed the entrepreneurial path, which focuses on creating a product or solution with a computing core and building a business around it.

The idea emerged from a relevant context in Brazil, where financial literacy remains low—only 35% of the population demonstrates basic knowledge of financial concepts (OECD, 2020)—and complex financial products often contribute to over-indebtedness. Managing personal finances is also a repetitive and time-consuming task, and traditional financial apps are not always as practical or engaging as a simple message-based interaction. Given the high penetration of messaging platforms like WhatsApp—installed on over 98% of smartphones in the country (DataReportal, 2024)—there is a clear opportunity to deliver accessible and effective financial guidance through a more familiar and user-friendly format.

## 2. Business description

The proposed business consists of a personal AI assistant that analyzes individual financial data and communicates insights through a messaging-based interface. The solution aims to deliver clear, concise, and actionable advice on personal finances using natural language, helping users better understand their spending, plan ahead, and improve their financial habits.

By integrating with platforms users already engage with daily, such as WhatsApp, the assistant minimizes friction and meets people where they are. The business leverages conversational AI to offer an intuitive and low-effort alternative to traditional apps, making personal finance management more accessible—especially for users with limited time, financial knowledge, or motivation to engage with complex tools.

## 3. Artifacts

At the beginning of the module, a backlog was created to guide the work over the 10-week period. However, as is often the case, the need for replanning emerged along the way. The following sections outline the discrepancies between the initial plan and the actual deliverables, along with brief descriptions of each artifact produced.

### 3.2. Developed artifacts

#### 3.2.1. TAPI and Project Plan

The opening documentation was developed to organize initial thoughts and establish the foundational structure of the project. It included key planning elements such as the product backlog, value proposition, and business premises. This stage was essential for outlining the project's first steps and setting long-term development goals, while maintaining the flexibility necessary to adapt to the project's evolving needs.

#### 3.2.2. Application Architecture

Although not explicitly listed in the product backlog, planning the application architecture proved to be one of the most critical steps before initiating development. The initial architectural proposal was a monolithic structure responsible for all backend processes and communication. However, upon further reflection, it became evident that this approach lacked a clear direction and required a level of planning that had not yet been achieved—particularly given that the system’s features were still poorly defined (and remain so to some extent). At that stage, the only concrete plan was the definition of the MVP’s core functionalities.

Consequently, the architecture was reconsidered. A new, highly granular design was proposed, consisting of multiple applications with distinct responsibilities. This structure aimed to maximize flexibility across the entire system. However, this approach introduced new challenges: the more applications involved, the greater the maintenance burden, the more complex the management of different environments, and the heavier the overall workload required to ensure cohesion.

Ultimately, a balanced architectural solution was developed—granular, yet not excessively so. This final design successfully separates core responsibilities while remaining practical, feasible to implement, and aligned with the project's flexibility goals.

#### 3.2.3. Low Fidelity Prototype

Before initiating the development tasks, a proof of concept was required to demonstrate the viability of the project using the selected AI provider and model. Initial testing yielded promising results, indicating the model's potential, although further refinements were still necessary to enhance its performance and and ensure consistent, standardized outputs.

#### 3.2.4. AInalytics API

The API, the primary and sole coding artifact developed in this module, is responsible for handling all prompting and result processing by interfacing with an external generative AI provider.

By implementing it as an independent application module rather than integrating it directly into a larger system, the API remains flexible, allowing for future scalability and potential adjustments regarding both consumers and providers.

#### 3.2.5. Product Development Plan and Product Benchmarking

These two steps were essential for identifying other players in the market and comparing their features. This market mapping process helped clarify and validate some of the project's premises and objectives, as well as highlight potential weaknesses and opportunities. However, it did not result in a complete SWOT analysis, as the project's strengths have not yet been fully defined or developed.

The product benchmarking focused on one player in particular using the same platform as the project plans to. After some testing, the results were also able to provide a clear vision to prevent unwanted use cases and clarify the differentials of the product under development.

## 4. Conclusion

The project demonstrated promising potential through early prototyping and initial AI integration. However, it faced key challenges in planning, time allocation, and execution. Several issues must be addressed to ensure the project's viability and scalability moving forward:

- Replicability: The current structure lacks standardized processes, making it difficult to replicate or scale reliably.
- Data consistency: Variations in data formatting and classification may affect the accuracy of the AI analysis.
- AI hallucination: The use of generative AI introduces the risk of unreliable or fabricated outputs, which can compromise trust.
- Planning gaps: The initial planning was underdeveloped, resulting in misaligned priorities and missed milestones.
- Developer availability: Limited time commitment from the developer hampers progress and delays key development phases.
- Manual transaction categorization: The inability for users to edit categories may lead to misclassifications and user dissatisfaction.
- Response time: Delays in delivering AI responses reduce user experience and can impact engagement.
- Addressing these issues will be essential for advancing the solution from a promising prototype to a functional and reliable financial tool.

## 5. References

DATAREPORTAL. Digital 2024: Brazil. 2024. Disponível em: https://datareportal.com/reports/digital-2024-brazil. Acesso em: 11 abr. 2025.

OECD. OECD/INFE international survey of adult financial literacy. Paris: OECD Publishing, 2020. Disponível em: https://www.oecd.org. Acesso em: 10 abr. 2025.

