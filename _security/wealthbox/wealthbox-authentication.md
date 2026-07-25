---
api_key_in:
- header
api_specs:
- filename: wealthbox-activity-api-openapi.yml
  format: yaml
  label: Wealthbox Activity API
  slug: wealthbox-activity-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wealthbox/refs/heads/main/openapi/wealthbox-activity-api-openapi.yml
- filename: wealthbox-contacts-api-openapi.yml
  format: yaml
  label: Wealthbox Contacts API
  slug: wealthbox-contacts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wealthbox/refs/heads/main/openapi/wealthbox-contacts-api-openapi.yml
- filename: wealthbox-events-api-openapi.yml
  format: yaml
  label: Wealthbox Events API
  slug: wealthbox-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wealthbox/refs/heads/main/openapi/wealthbox-events-api-openapi.yml
- filename: wealthbox-notes-api-openapi.yml
  format: yaml
  label: Wealthbox Notes API
  slug: wealthbox-notes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wealthbox/refs/heads/main/openapi/wealthbox-notes-api-openapi.yml
- filename: wealthbox-opportunities-api-openapi.yml
  format: yaml
  label: Wealthbox Opportunities API
  slug: wealthbox-opportunities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wealthbox/refs/heads/main/openapi/wealthbox-opportunities-api-openapi.yml
- filename: wealthbox-profile-api-openapi.yml
  format: yaml
  label: Wealthbox Profile API
  slug: wealthbox-profile-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wealthbox/refs/heads/main/openapi/wealthbox-profile-api-openapi.yml
- filename: wealthbox-tasks-api-openapi.yml
  format: yaml
  label: Wealthbox Tasks API
  slug: wealthbox-tasks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wealthbox/refs/heads/main/openapi/wealthbox-tasks-api-openapi.yml
- filename: wealthbox-teams-api-openapi.yml
  format: yaml
  label: Wealthbox Teams API
  slug: wealthbox-teams-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wealthbox/refs/heads/main/openapi/wealthbox-teams-api-openapi.yml
- filename: wealthbox-users-api-openapi.yml
  format: yaml
  label: Wealthbox Users API
  slug: wealthbox-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wealthbox/refs/heads/main/openapi/wealthbox-users-api-openapi.yml
- filename: wealthbox-workflows-api-openapi.yml
  format: yaml
  label: Wealthbox Workflows API
  slug: wealthbox-workflows-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wealthbox/refs/heads/main/openapi/wealthbox-workflows-api-openapi.yml
auth_types:
- apiKey
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Wealthbox Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Wealthbox secures its APIs with apiKey and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Wealthbox
provider_slug: wealthbox
scheme_count: 2
schemes:
- description: Personal Access Token issued from the Wealthbox account settings.
  in: header
  name: accessToken
  parameter: ACCESS_TOKEN
  sources:
  - openapi/wealthbox-openapi.yml
  type: apiKey
- description: OAuth 2.0 authorization code flow for third-party integrations.
  flows:
  - authorizationUrl: https://app.crmworkspace.com/oauth/authorize
    flow: authorizationCode
    scopes: 2
    tokenUrl: https://app.crmworkspace.com/oauth/token
  name: oauth2
  sources:
  - openapi/wealthbox-openapi.yml
  type: oauth2
slug: wealthbox-authentication
source_filename: wealthbox-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/wealthbox-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - oauth2\n  api_key_in:\n  - header\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: accessToken\n  type: apiKey\n  in: header\n  parameter: ACCESS_TOKEN\n  description: Personal Access Token issued from the Wealthbox account settings.\n  sources:\n  - openapi/wealthbox-openapi.yml\n- name: oauth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://app.crmworkspace.com/oauth/authorize\n    tokenUrl: https://app.crmworkspace.com/oauth/token\n    scopes: 2\n  description: OAuth 2.0 authorization code flow for third-party integrations.\n  sources:\n  - openapi/wealthbox-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/wealthbox/refs/heads/main/authentication/wealthbox-authentication.yml
summary_line: apiKey/oauth2 · 2 schemes
tags:
- CRM
- Financial Advisors
- Wealth Management
- Contact Management
- Workflow Automation
- SaaS
---
