# ARGUS — System Requirements

## 1. Purpose

This document defines the initial functional and non-functional requirements of the ARGUS Flash Flood Alert System for Bagh district, Azad Kashmir, Pakistan.

## 2. Functional Requirements

### FR-01: Interactive Map
The system shall display an interactive map of the selected study area using Leaflet.js and OpenStreetMap.

### FR-02: Flood-Prone Channel Visualization
The system shall load and display predefined flood-prone channels using GeoJSON data.

### FR-03: Rainfall Forecast Integration
The backend shall retrieve rainfall forecast data for the selected region using the Open-Meteo API.

### FR-04: Forecast Refresh
The system shall refresh forecast data at a configurable interval.

### FR-05: Threshold-Based Risk Assessment
The system shall compare relevant forecast rainfall values against agreed danger thresholds and classify potentially hazardous channels.

### FR-06: Alert Visualization
The map shall visually distinguish channels that meet the configured risk criteria.

### FR-07: Data Storage
The backend shall use MySQL to store the relevant channel records, forecast data, and alert status, subject to the final database design.

### FR-08: Data Source Documentation
The project shall document the sources, assumptions, and methodology used to identify flood-prone channels.

## 3. Non-Functional Requirements

### NFR-01: Usability
The map and alerts should be understandable to users with basic computer skills.

### NFR-02: Maintainability
The frontend, backend, geographic data, and database components should be organized for easier maintenance.

### NFR-03: Reliability
The system should handle unavailable forecast data or API errors without displaying stale information as if it were current.

### NFR-04: Data Integrity
Geographic data and rainfall values should be validated before being used for risk assessment.

### NFR-05: Security
Database credentials and other sensitive configuration values shall not be committed to the public repository.

## 4. Requirements Requiring Further Decisions

The following details must be agreed upon and documented before finalizing the alert mechanism:

- Rainfall thresholds and their units.
- Rainfall accumulation period used for assessment.
- Method for associating forecast locations with individual channels.
- Forecast refresh interval.
- Criteria for classifying alert severity.
- Data sources and validation method for the channel dataset.

## 5. Limitations

ARGUS uses forecast rainfall and predefined geographic data. Its output represents potential risk, not a guarantee that flooding will or will not occur. The system is not a substitute for official emergency warnings.

## 6. Status

Initial draft — requirements are subject to review and approval by the project team and requirements provider.
