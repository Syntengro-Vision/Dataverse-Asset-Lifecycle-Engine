# Dataverse-Asset-Lifecycle-Engine
A CMMC-aligned Power Platform framework for hardware lifecycle management, integrating Entra ID identity mapping with automated maintenance auditing.


Overview
This repository contains the architecture for a Model-Driven App designed to solve "Helpdesk Fatigue" in IT asset management.

Key Features
Identity-Linked Assets: Replaces text-based entry with relational Lookups to Entra ID (Users) for non-repudiable audit trails.

Automated "Circuit Breaker": A Power Automate engine that distinguishes between routine maintenance (Silent Audit) and break/fix failures (Active Ticket).

CMMC Alignment: Specifically maps to AU.L2-3.3.1 (Audit Generation) and AM.L2-3.1.1 (Asset Management).
