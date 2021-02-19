# GitHub Team Hack

## Introduction

The goal of the hack is to go through various scenarios defined below and to share learnings. 

The outcome of each scenario will depend on the specific scenario, but should be one of the following:

* Learning about the various SKUs of GitHub and their capabilities.
* Documentation (stored on this repo as MD files).
* Sample/code references.
* Feedback for GitHub Engineering.

## Pre-Requisites

* Set up GitHub Enterprise 3.x RC server for use
  
  * We will have a server VM ready for folks to use if their scenario doesn't include install or they would like to jump into their scenario (ie security)

  * Folks can still provision their own GHE VM and for folks focused on Scenario 3, it's recommended they go through the install process.

* Define Target Azure Sub and provision SP's.
* Confirm Teams and adjust as needed.
* Teams/Participants register for Enterprise cloud and server licenses.
[https://msftghes.azurewebsites.net/](https://msftghes.azurewebsites.net/)
* Schedule Post Hack Followup meeting:
  * 1 hour team meeting after hack to discuss findings.
  * Demo : 10 mins per scenario/team

## Team Structure

The teams were allocated randomly, mixing folks form Richard and David's teams. Each team consists of two engineers, with the exception of team 5. We grouped David with Dariusz and Engin as they were are on different time zones and could take turns pairing with David with David throughout the day.

### Team 1

* Brian
* Richard

### Team 2

* Sushant
* Brent

### Team 3

* Tom
* Hadwa

### Team 4

* Eugene
* Hattan

### Team 5

* David
* Dariusz
* Engin

## Proposed Schedule

This is a rough schedule, folks can adjust as needed.

| Time               | Description   |
| ------------------ | ------------- |
| 09:00am - 09:30am  | Kickoff       |
| 09:30am - 12:00pm  | hacking       |
| 12:00pm - 01:00pm  | Lunch         |
| 01:00pm - 01:15pm  | Team Check-in |
| 01:15pm - 05:00pm  | hacking       |

## Scenarios

### 1. Secrets Management & Rotation

* KeyVault integration vs Repo Secrets
* PAT generation and rotation

### 2. Security Scanning and Alerting

* Security and Key Scanning on GHE Server
* Pick up secrets on check-in
* Pre-commit hooks
* Will refs still be pullable for secrets checked in ?
* Dependabot alerts for CVE Scanning across all SKUs

## 3. Orchestration & Set UP

* Enterprise Server with Cloud Connections (Hybrid Test Drive)
* Enterprise Server with Hosted Agents (Hybrid Test Drive)
* Arm / Terraform template for GHE Server 3.0.0 RC

## 4. Feature Parity , Documentation & Examples

* Differences between GH SKUs (Public, Enterprise Cloud and Enterprise Server)
* General Actions Support on GHE Server
* Do Codespaces work on GHE Server ?
* API Differences between the SKUs ( Are all the endpoints represented )
* GH CLI support across all SKUs
* Github Packages (Private Packages not shared with the general public)
* GH Mobile and Desktop App support across all SKUs (Apps - GitHub Docs)

## 5. Observability/Enterpriseness

* Alerting: What are the options ?
* Enterprise Auditing
* What tooling is there available for monitoring, metrics and visualization( Azure Monitor, Prometheus, etc )
* HA/DR for GHE Server
* GHE Server in a disconnected/ air-gapped environment

## Test Harness Projects

* DevOps OpenHack - [https://github.com/azure-samples/openhack-devops-team/tree/openhack_refresh](https://github.com/azure-samples/openhack-devops-team/tree/openhack_refresh)

* DevSecOps OpenHack - [https://dev.azure.com/cseeest/OpenHack/_git/DevSecOps_Light](https://dev.azure.com/cseeest/OpenHack/_git/DevSecOps_Light)

