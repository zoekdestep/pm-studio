# Technical Context

This file helps PM Studio understand technical constraints and architecture. It ensures specs are grounded in reality.

**This file is optional.** If you have existing technical documentation, you can ask Claude to fill this out by saying: *"Here's our technical spec [paste or upload]. Please fill out technical-context.md based on this."*

---

## Architecture Overview

### High-Level Architecture

[Describe your system architecture at a high level - what are the main components and how do they interact?]

### Key Components

| Component | What It Does | Owner |
|-----------|--------------|-------|
| [Component 1] | [Description] | [Team] |
| [Component 2] | [Description] | [Team] |

### Data Flow

[Describe how data flows through your system for key scenarios]

---

## Platforms

### [Platform 1, e.g., Web]

- **Tech stack:** [Technologies used]
- **Deployment:** [How updates ship]
- **Constraints:** [Platform-specific limitations]

### [Platform 2, e.g., Mobile]

- **Tech stack:** [Technologies used]
- **Deployment:** [How updates ship]
- **Constraints:** [Platform-specific limitations]

---

## Key Services & Dependencies

### Core Services

| Service | What It Does | Latency | Cost Considerations |
|---------|--------------|---------|---------------------|
| [Service 1] | [Description] | [Target] | [Notes] |

### Data Services

| Service | What It Does | Limitations |
|---------|--------------|-------------|
| [Service 1] | [Description] | [Limitations] |

---

## Common Technical Constraints

### Performance

- **Latency budget:** [Target response times]
- **Success rate targets:** [Target %]
- **Known bottlenecks:** [Current issues]

### Scale

[Scale considerations for your system]

### Security & Compliance

[Relevant security constraints]

---

## Integration Points

### Internal Integrations

| System | Integration Type | Notes |
|--------|------------------|-------|
| [System 1] | [Type] | [Details] |

### External Integrations

| System | Integration Type | Notes |
|--------|------------------|-------|
| [System 1] | [Type] | [Details] |

---

## Feature Flags & Experimentation

### How Features Ship

- **Stages:** [Your rollout stages]
- **Experiment framework:** [How you run experiments]

---

## Technical Debt & Known Issues

| Issue | Impact | Status |
|-------|--------|--------|
| [Issue 1] | [How it affects users/team] | [Current status] |

---

## Engineering Team Structure

| Team | Owns | Key Contact |
|------|------|-------------|
| [Team 1] | [Ownership area] | [Contact] |

---

## Glossary (Technical)

| Term | Definition |
|------|------------|
| [Term 1] | [Definition] |
