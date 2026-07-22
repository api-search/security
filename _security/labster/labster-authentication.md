---
api_key_in: []
auth_types:
- openIdConnect
- oauth2
- password
description: ''
kind: authentication
layout: security
method: searched
name: Labster Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
- jwtBearer
overview: Labster secures its APIs with openIdConnect, oauth2, and password across 5 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials and jwtBearer flow(s).
provider_name: Labster
provider_slug: labster
scheme_count: 5
schemes:
- description: Primary institutional integration. The LMS registers Labster as an LTI 1.3 tool using a developer key / client ID, and launches students into Labster via the OIDC third-party-initiated login flow. Endpoint configuration (tool JSON URL, client ID) is issued per customer by a Labster Customer Success Manager and is not published publicly.
  docs: https://help.labster.com/en/collections/3094279-lms-integration-for-lms-admin
  name: LTI 1.3 launch
  platforms:
  - Canvas
  - Blackboard
  - Blackboard Ultra
  - Moodle
  - D2L Brightspace
  - Sakai
  - Schoology
  standard: 1EdTech LTI 1.3
  type: openIdConnect
- description: District users authenticate through their Clever Portal and are redirected into the Labster Course Manager. Identity is matched on the student email address linked to the Clever account. Rostering / Clever Secure Sync is not documented; instructors invite students by email.
  docs: https://help.labster.com/en/articles/11971470-accessing-labster-through-labster-s-clever-integration
  name: Clever SSO
  type: openIdConnect
- description: Direct email/password sign-in to the Labster course manager.
  in: https://my.labster.com/
  name: Labster account login
  type: password
- description: Service-to-service authentication between Labster's own backend services, as implemented in the open-source Livit/Labster.OAuth2Client library. Not exposed to third-party developers.
  flow: clientCredentials
  name: OAuth2 client credentials (internal)
  source: https://github.com/Livit/Labster.OAuth2Client
  type: oauth2
- description: Used by Labster for communication with Salesforce, per the Labster.OAuth2Client documentation. Not exposed to third-party developers.
  flow: jwtBearer
  name: JWT Bearer grant (internal)
  source: https://github.com/Livit/Labster.OAuth2Client
  standard: RFC 7523
  type: oauth2
slug: labster-authentication
source_filename: labster-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: https://help.labster.com/en/collections/3094279-lms-integration-for-lms-admin\ndocs: https://help.labster.com/en/collections/681668-access-to-labster\nnote: >-\n  Derived from documentation rather than an OpenAPI securitySchemes block, because\n  Labster ships no public API. Authentication here describes how users and LMS\n  platforms authenticate into the Labster product surface.\nsummary:\n  types:\n  - openIdConnect\n  - oauth2\n  - password\n  api_key_in: []\n  oauth2_flows:\n  - clientCredentials\n  - jwtBearer\n  public_api: false\nschemes:\n- name: LTI 1.3 launch\n  type: openIdConnect\n  standard: 1EdTech LTI 1.3\n  description: >-\n    Primary institutional integration. The LMS registers Labster as an LTI 1.3\n    tool using a developer key / client ID, and launches students into Labster via\n    the OIDC third-party-initiated login flow. Endpoint configuration (tool JSON\n    URL, client ID) is issued per customer\
  \ by a Labster Customer Success Manager\n    and is not published publicly.\n  platforms:\n  - Canvas\n  - Blackboard\n  - Blackboard Ultra\n  - Moodle\n  - D2L Brightspace\n  - Sakai\n  - Schoology\n  docs: https://help.labster.com/en/collections/3094279-lms-integration-for-lms-admin\n- name: Clever SSO\n  type: openIdConnect\n  description: >-\n    District users authenticate through their Clever Portal and are redirected\n    into the Labster Course Manager. Identity is matched on the student email\n    address linked to the Clever account. Rostering / Clever Secure Sync is not\n    documented; instructors invite students by email.\n  docs: https://help.labster.com/en/articles/11971470-accessing-labster-through-labster-s-clever-integration\n- name: Labster account login\n  type: password\n  in: https://my.labster.com/\n  description: Direct email/password sign-in to the Labster course manager.\n- name: OAuth2 client credentials (internal)\n  type: oauth2\n  flow: clientCredentials\n\
  \  description: >-\n    Service-to-service authentication between Labster's own backend services, as\n    implemented in the open-source Livit/Labster.OAuth2Client library. Not exposed\n    to third-party developers.\n  source: https://github.com/Livit/Labster.OAuth2Client\n- name: JWT Bearer grant (internal)\n  type: oauth2\n  flow: jwtBearer\n  standard: RFC 7523\n  description: >-\n    Used by Labster for communication with Salesforce, per the Labster.OAuth2Client\n    documentation. Not exposed to third-party developers.\n  source: https://github.com/Livit/Labster.OAuth2Client\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/labster/refs/heads/main/authentication/labster-authentication.yml
summary_line: openIdConnect/oauth2/password · 5 schemes
tags:
- Company
- Education
- EdTech
- Virtual Labs
- Science Education
- STEM
- Simulation
- Learning Management System
- LTI
- Higher Education
---
