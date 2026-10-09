# ARGUS — Development Plan

## 1. Introduction

This document describes the planned development process for the ARGUS Flash Flood Alert System. The project will follow an Agile, iterative, Scrum-inspired methodology, as described in the project proposal.

Development will proceed in small increments, allowing the team to review progress, test features, and incorporate feedback from the requirements provider (RP).

## 2. Development Objectives

- Develop an interactive map of Bagh district, Azad Kashmir.
- Display predefined flood-prone channels using GeoJSON.
- Integrate rainfall forecast data from the Open-Meteo API.
- Implement threshold-based hazard classification.
- Display potential hazards on the map.
- Test and document the integrated system.

## 3. Development Phases

### Phase 1: Planning and Requirements

Activities:
- Review the project proposal.
- Finalize functional and non-functional requirements.
- Identify project risks and dependencies.
- Assign responsibilities to team members.
- Create GitHub issues and a project board.

Expected outcome: An agreed requirements document and an organized development backlog.

### Phase 2: Research and Analysis

Activities:
- Research flood-prone channels in Bagh district.
- Identify reliable geographic data sources.
- Explore the Open-Meteo forecast API.
- Investigate suitable rainfall thresholds and assessment periods.
- Document assumptions and limitations.

Expected outcome: Documented data sources and an initial approach to hazard assessment.

### Phase 3: System Design

Activities:
- Design the web interface and map layout.
- Plan the frontend and backend architecture.
- Design the GeoJSON data structure.
- Plan the MySQL database schema.
- Design the alert visualization.

Expected outcome: Initial system design and interface mockups.

### Phase 4: Implementation

Development will take place incrementally.

**Increment 1 — Map Interface**
- Build the initial web interface.
- Integrate Leaflet.js and the OpenStreetMap base map.

**Increment 2 — Hazard Data**
- Prepare the researched flood-channel dataset.
- Load and display GeoJSON channels on the map.

**Increment 3 — Weather Integration**
- Connect the Flask backend to the Open-Meteo API.
- Retrieve and validate forecast rainfall data.

**Increment 4 — Alert Mechanism**
- Implement the agreed rainfall threshold rules.
- Classify potentially hazardous channels.
- Display alert status on the map.

**Increment 5 — Data Storage and Integration**
- Implement the required MySQL tables.
- Integrate the frontend, backend, and database.

Expected outcome: An integrated application implementing the agreed project scope.

### Phase 5: Testing

Activities:
- Test map rendering and GeoJSON loading.
- Test weather API responses and error handling.
- Test rainfall threshold calculations.
- Test database operations.
- Perform integration testing.
- Record defects and their resolutions.

Expected outcome: Documented test results and a more reliable integrated application.

### Phase 6: Final Delivery

Activities:
- Review the completed requirements.
- Update project documentation.
- Prepare a demonstration.
- Document known limitations.
- Prepare the final academic presentation.

Expected outcome: A documented academic project ready for demonstration and evaluation.

## 4. Team Collaboration

The team will use GitHub for source control and task tracking.

- GitHub Issues will record tasks and defects.
- A project board will track work as To do, In progress, and Completed.
- Feature branches will be used for independent development.
- Pull requests will be used to review changes before merging into the main branch.
- Weekly team meetings will review progress and blockers.
- Monthly meetings with the requirements provider will gather feedback.

## 5. Progress Monitoring

Progress will be evaluated by reviewing completed tasks, testing results, unresolved issues, and feedback from the requirements provider.

Meeting decisions and agreed changes will be recorded in `docs/meetings/`.

## 6. Change Management

Proposed changes will be reviewed by the team and requirements provider. Each change will be evaluated against the project scope, available time, technical feasibility, and expected effort.

Approved changes will be added to the development backlog.

## 7. Risks and Limitations

- Reliable flood-channel data may be difficult to obtain.
- Forecast rainfall may not accurately represent conditions at an individual channel.
- Suitable rainfall thresholds require research and validation.
- External API availability may affect the system.
- The project timeline may require adjustments as technical challenges arise.

## 8. Status

This is an initial development plan based on the project proposal. Detailed dates, iteration durations, and task assignments will be agreed upon by the team.
