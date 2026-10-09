# ARGUS — Project Overview

## 1. Introduction

ARGUS is a proposed academic flash flood alert system focused on Bagh District, Azad Jammu and Kashmir. The project aims to support local flood-risk awareness by connecting forecasted rainfall with known flood-prone seasonal stream channels, locally referred to as *nala*.

In mountainous regions, steep terrain and intense rainfall can cause water to flow rapidly through stream channels. These channels may remain dry during periods without rain but can become hazardous during heavy rainfall. Because such channels may not be monitored in the same way as major rivers, rainfall forecasts alone may not provide sufficiently location-specific information about potential hazards.

ARGUS proposes an interactive, map-based approach to help visualize known flood-prone channels alongside forecast rainfall information. By applying defined rainfall thresholds, the system aims to identify channels that may warrant attention under forecast conditions.

## 2. Problem Statement

The central problem addressed by ARGUS is the lack of a direct connection between rainfall forecasts and known flood-prone ephemeral stream channels in the selected study area.

Although rainfall forecasts can indicate potentially hazardous weather, they do not automatically identify which mapped seasonal channels may be at risk. This information gap can make it difficult for people and relevant authorities to understand where forecast rainfall may create localized concerns, particularly in mountainous areas and along mountain roads.

ARGUS proposes to address this gap by combining researched channel data, rainfall forecasts, and threshold-based alert logic within a single web-based mapping interface.

## 3. Project Objectives

The main objectives of ARGUS are:

* To develop an interactive map of Bagh District, Azad Jammu and Kashmir.
* To represent pre-identified, researched flood-prone channels as a GeoJSON hazard layer.
* To integrate forecast rainfall information for the selected region through a weather API and refresh forecast values at regular intervals while the system is running.
* To implement a threshold-based warning mechanism that flags mapped channels when forecast rainfall meets or exceeds defined danger thresholds.
* To visualize potential alerts on the map to support localized flood-risk awareness.
* To document the data sources and methodology used to identify and represent flood-prone channels.

## 4. Project Scope

### 4.1 In Scope

The proposed project includes:

* A web-based interactive map for Bagh District.
* A researched, predefined dataset of flood-prone ephemeral stream channels represented in GeoJSON format.
* Integration of rainfall forecasts from a weather API.
* Threshold-based evaluation of forecast rainfall associated with mapped channels.
* Map-based visualization of potential alerts.
* A backend component for managing hazard-channel data, retrieving and refreshing forecast information, and evaluating alert conditions.
* Documentation of the data sources and methodology used to identify the selected channels.

### 4.2 Out of Scope

The following features are excluded from the current project scope:

* Automatic discovery of new flood channels using satellite imagery, remote sensing, or computer vision.
* Expansion of the system to additional districts or regions.
* Integration with physical water-level sensors or IoT devices.
* Development of a dedicated mobile application.
* Direct integration with national or regional disaster-management systems, including NDMA or PDMA platforms.
* SMS and push-notification services. The proposed alerts are intended to be presented through the application's interface; external notifications may be considered in future versions.

## 5. Stakeholders

The proposed system identifies the following stakeholders:

* **Local disaster-management authorities:** Potential primary users who could review mapped hazards and forecast-based alerts when assessing local risks.
* **Residents of flood-prone areas:** Potential indirect beneficiaries of improved local risk awareness and any advisories issued by relevant authorities.
* **Travellers and tourists:** Potential indirect beneficiaries of route advisories informed by local risk assessments.
* **Requirement provider:** The project stakeholder who helps define requirements, reviews the system's design and alert logic, and provides feedback during development.
* **Development team:** The four-student team responsible for researching the hazard data, designing and implementing the system, testing its components, and maintaining the documentation.
* **Course instructor:** The academic supervisor responsible for assessing the project proposal, implementation, and learning outcomes against course requirements.

These are proposed stakeholder roles; they do not imply that the system has been adopted by any authority.

## 6. Software Development Methodology

ARGUS proposes an iterative, Agile development approach inspired by Scrum. This approach is suitable for the project because requirements, hazard-data sources, and alert thresholds may need refinement as the team conducts research and develops its understanding of the problem.

Development is planned in increments, allowing individual components to be designed, implemented, reviewed, and tested progressively.

The planned phases are:

1. **Planning:** Define objectives, scope, team responsibilities, and development tasks.
2. **Analysis:** Gather requirements, research flood-prone channels in Bagh, investigate weather-data sources, and define an approach to risk thresholds.
3. **Design:** Develop the system architecture, database design, map interface, and alert-view mockups.
4. **Implementation:** Build the system incrementally, developing one feature group at a time.
5. **Testing:** Test individual components as they are developed and perform integration tests using appropriate rainfall scenarios.
6. **Delivery:** Demonstrate completed increments and prepare the final integrated system and academic presentation.

The team plans to hold weekly meetings to review progress, discuss difficulties, and update task status. Periodic reviews with the requirement provider will be used to collect feedback and determine appropriate changes. Decisions, feedback, and agreed actions will be recorded in meeting minutes.

The four team members will initially explore the proposed modules: map development, user-interface development, flood-channel data, and documentation and testing. Final responsibility assignments will be determined as the team gains experience and evaluates individual interests and capabilities. Team members are expected to understand the overall system, even when they have individual module responsibilities.

## 7. Proposed Tools and Technologies

The project proposal identifies the following tools and technologies:

| Tool or technology    | Intended purpose                                                           |
| --------------------- | -------------------------------------------------------------------------- |
| HTML, CSS, JavaScript | Development of the web interface                                           |
| Leaflet.js            | Interactive mapping and display of flood-channel layers                    |
| OpenStreetMap         | Base-map data and geographic context                                       |
| GeoJSON               | Representation of flood-channel geometries                                 |
| QGIS and geojson.io   | Geographic data preparation, channel tracing, and GeoJSON export           |
| Open-Meteo API        | Retrieval of rainfall forecast information for the Bagh region             |
| Python with Flask     | Backend services, forecast retrieval, and threshold-based alert evaluation |
| MySQL                 | Storage of channel data, forecast records, and alert status                |
| Figma                 | Interface mockups and design                                               |
| Git and GitHub        | Version control, team collaboration, and project tracking                  |
| Visual Studio Code    | Code editing and development                                               |

These technologies represent the proposed stack and may be refined as development progresses.

## 8. Limitations and Responsible Use

ARGUS is an academic project intended to explore the relationship between forecast rainfall and known flood-prone channels in a defined geographical area. Its usefulness will depend on the quality and coverage of the channel dataset, the availability and accuracy of forecast information, and the suitability of the thresholds selected by the team.

A threshold-based alert indicates a potential concern under the system's configured rules; it does not confirm that a flood will occur. The proposed system does not directly measure water levels and is not intended to replace official forecasts, emergency instructions, or professional assessments.

ARGUS should therefore be treated as an academic prototype for flood-risk awareness, not as an officially certified operational warning service.

## 9. Current Project Status

This repository is being used to organize the project proposal, meeting records, technical documentation, development work, and testing evidence.

The features and technologies described in this overview are based on the project proposal. They should not be interpreted as completed or verified implementation. This section should be updated as development progresses, with completed features and test results documented only after they have actually been implemented and evaluated.

## 10. References

The final academic report should include the sources consulted for the flood-risk background, regional information, geographic data, rainfall forecasts, and technical tools. References and in-text citations should follow the IEEE referencing style required by the project guidelines.

The final reference list should be completed using the sources actually consulted and cited by the team.
