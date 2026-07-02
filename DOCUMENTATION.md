---
title: Documentation
permalink: /documentation/
---

# Team Health and Personality Assessment for Jira

## Overview

Team Health and Personality Assessment for Jira helps teams review workplace collaboration, work-style preferences, and team-level health indicators inside Jira. The app provides Big Five, DISC, and MBTI-compatible questionnaires, individual result pages, aggregate team analytics, and executive-level filters for organization-wide review.

The app is designed for workplace insight, coaching, communication planning, and team support. It is not intended for clinical diagnosis, medical assessment, hiring decisions, performance scoring, or automated employment decisions.

## Installation

1. Install the app from Atlassian Marketplace or through an approved Forge installation link.
2. Confirm the requested Jira scopes during installation.
3. Open Jira and go to **Apps**.
4. Select **Team Health Assessment**.
5. Jira administrators can open the app from Jira administration settings to configure privacy and reassessment options.

After installation, users can access the app from the Jira Apps menu. Administrators can configure the minimum privacy threshold, reassessment interval, and named-result visibility policy.

## User Roles

The app displays pages based on Jira groups and administrative access.

| Role | Typical Jira group | Main access |
| --- | --- | --- |
| Participant | Standard Jira user | My Results, Answer Questions |
| PM | `pm` | PM panel and team analytics |
| PO | `po` | PO panel and team analytics |
| Project Manager | `project manager` | PM guidance and team analytics |
| HR Manager | `hrmanage` | HR panel and privacy-aware organization analytics |
| Executive Officer | `executive officer` or `executive` | Executive filters and organization-level views |
| Jira Administrator | Jira/site admin | Settings, analytics, HR, Executive, and Marketplace hardening pages |

Group names can be adjusted by the Jira administrator as part of the site access model.

## My Results

The **My Results** page gives each user a personal summary of their latest assessment results.

Users can see:

- Big Five workplace signal
- DISC workstyle signal
- MBTI-compatible preference pattern
- Reassessment schedule
- Last answered date
- Next allowed reassessment date
- Work pressure and collaboration trend summary

Personal results are intended to help users reflect on work style, communication preferences, and collaboration habits.

## Answer Questions

The **Answer Questions** page allows users to complete the available assessment questionnaires.

Available models:

- Big Five-compatible questionnaire
- DISC-compatible questionnaire
- MBTI-compatible questionnaire

Administrators can configure how often users are allowed or required to reassess. Until the next allowed reassessment date, the questionnaire is locked and the user is shown when they can answer again.

Only the latest raw answer set is kept for each user and model. Computed result snapshots may be retained with timestamps to support trend views.

## Team Analytics

The **Team Analytics** page shows aggregate results for authorized users.

Team analytics may include:

- Response coverage
- Privacy threshold status
- MBTI distribution
- User personality index
- Aggregate team-level signals

When privacy thresholds are not met, small groups are hidden to reduce the risk of identifying individuals.

## Executive Filters

The **Executive** page is designed for organization-level review and planning. It compares team outputs and collaboration signals without judging individuals.

Available filters include:

- Scope
- Project
- Team
- Role
- Test type: Big Five, DISC, or MBTI
- Pressure level

Executive charts update based on the selected test type and filters. For example, switching from MBTI to Big Five changes the chart titles, labels, and grouped values to match Big Five results.

Executive analytics are intended for organizational support, capacity planning, and team-level insight. They must not be used for direct individual evaluation, hiring decisions, or clinical interpretation.

## Privacy And Responsible Use

The app uses privacy thresholds to prevent small-group analytics from exposing identifiable results. Administrators can configure the minimum number of completed responses required before aggregate charts are shown.

Security and privacy details are available here:

https://github.com/misaqyrn2019/TeamHealthApps/blob/main/SECURITY_PRIVACY.md

Responsible use principles:

- Use results as workplace and collaboration indicators only.
- Do not use results for medical or clinical diagnosis.
- Do not use results as a hiring, promotion, or disciplinary decision tool.
- Do not expose personal results unless authorized and appropriate.
- Review team-level results in context with workload, project conditions, and team structure.
- Keep access limited to users with a legitimate business need.

## Support Contact

For support, installation questions, privacy requests, or issue reports, use the repository issue tracker:

https://github.com/misaqyrn2019/TeamHealthApps/issues

For Marketplace installations, use the support contact listed in the Atlassian Marketplace app listing.
