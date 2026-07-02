# Security And Privacy

## What Data Is Collected

Team Health and Personality Assessment for Jira may collect and process the following app-specific data:

- Jira account identifier for the signed-in user
- Jira display name, when available from Jira
- Jira group and role-related information used for access control
- Latest questionnaire answers for Big Five, DISC, and MBTI-compatible models
- Computed assessment results, including primary type or workstyle signal
- Computed dimension scores and pressure/collaboration indicators
- Assessment completion timestamps
- App settings configured by Jira administrators
- Aggregate team-level analytics derived from completed assessments

The app is designed to collect only the information needed to provide individual results, role-aware views, reassessment scheduling, and aggregate analytics.

## Where Data Is Stored

App data is stored in Atlassian Forge Storage associated with the installed Forge app and Atlassian site. The app does not require an external database for its standard Cloud version.

Data remains within the Atlassian Forge platform storage layer for the installed app environment.

## How Forge Storage Is Used

Forge Storage is used for:

- App configuration settings
- The latest saved answer set per user and assessment model
- Computed result snapshots with timestamps
- User profile metadata needed for app access and analytics
- Aggregate-ready indexes used by team and executive views

Raw questionnaire answers are kept as the latest response for each user and model. Historical trend views use computed result snapshots and summary indicators rather than requiring every previous raw answer set.

## Who Can Access Personal And Team-Level Results

Access depends on Jira permissions, Jira groups, and the page being used.

Typical access model:

- Standard users can access their own results and questionnaires.
- PM and PO roles can access role-specific guidance and team-level views where allowed.
- HR users can access privacy-aware organization analytics.
- Executive users can access organization-level filters and aggregate views.
- Jira administrators can configure settings and review administrative pages.

Named individual summaries should only be visible when explicitly enabled by an administrator and when the user has an authorized HR, executive, or administrative role.

## How Privacy Thresholds Work

Privacy thresholds reduce the risk of exposing individual assessment results in small groups.

When a selected project, team, role, or filter scope has fewer completed responses than the configured threshold, aggregate charts are hidden. Instead of showing charts, the app displays a privacy message explaining that the selected scope is below the minimum response count.

This helps prevent small groups from being used to infer individual personality or pressure signals.

## How Data Is Protected

The app is built on Atlassian Forge and uses Forge platform controls for app execution and storage. Data protection practices include:

- Storing app data in Forge Storage
- Avoiding external storage for the standard Cloud version
- Using Jira and Forge permissions to control app access
- Applying privacy thresholds before showing aggregate analytics
- Limiting standard users to their own assessment results
- Avoiding clinical, hiring, or employment-decision labels in the product experience
- Keeping sensitive configuration and credentials out of source code

Site administrators are responsible for assigning Jira groups and roles appropriately and for limiting access to authorized users.

## How Users Can Request Deletion Or Support

Users can request support, data deletion, or privacy assistance through the repository issue tracker:

https://github.com/misaqyrn2019/TeamHealthApps/issues

For Marketplace installations, users should also use the support contact listed in the Atlassian Marketplace app listing.

Deletion requests should include enough information for the site administrator or support team to identify the relevant Jira site and user account. Do not include passwords, API tokens, private assessment answers, or other sensitive information in public issues.

## Not For Clinical Diagnosis Or Hiring Decisions

The app provides workplace wellbeing, work-style, collaboration, and team-level indicators. It does not provide medical, psychological, psychiatric, or clinical diagnosis.

The app must not be used as:

- A clinical diagnosis tool
- A medical assessment tool
- A hiring or rejection decision tool
- A promotion or compensation decision tool
- A disciplinary or performance scoring system
- An automated employment decision system

Results should be interpreted as supportive workplace signals and reviewed with context, care, and appropriate human judgment.
