---
api_key_in:
- dashboard-issued
auth_types:
- oauth2
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Axos Bank Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: Axos Bank secures its APIs with oauth2 and apiKey across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: Axos Bank
provider_slug: axos-bank
scheme_count: 2
schemes:
- description: OAuth 2.0 token-based authentication documented for the Axos API Store. Flow details, authorization/token URLs, and scopes are provisioned to onboarded partners and are not published publicly.
  documented_flow: clientCredentials
  name: OAuth2
  source: https://www.axosbank.com/developer
  type: oauth2
- description: API keys issued to each onboarded developer through a per-user secure developer dashboard, used alongside OAuth 2.0 tokens.
  in: dashboard-issued
  name: DeveloperDashboardKey
  source: https://www.axosbank.com/developer
  type: apiKey
slug: axos-bank-authentication
source_filename: axos-bank-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-23'\nmethod: searched\nsource: https://www.axosbank.com/developer\ndocs: https://www.axosbank.com/developer\nnote: >-\n  Axos Bank's developer / Banking-as-a-Service program documents OAuth 2.0\n  token-based authentication for its four API product families (Account\n  Enrollment, Account Maintenance, Payment Solutions, Account Reporting).\n  Access is partner-gated: a developer contacts the Axos API team, who\n  provision sandbox/test credentials and later production credentials, and API\n  keys are issued through a per-user secure developer dashboard. No public\n  OpenAPI specification is published, so no machine-readable securityScheme\n  could be harvested; this profile is captured from the public developer-portal\n  documentation. Token, authorization, and scope endpoints are disclosed only\n  after onboarding.\nsummary:\n  types:\n  - oauth2\n  - apiKey\n  api_key_in:\n  - dashboard-issued\n  oauth2_flows:\n  - clientCredentials\n  access_model: partner-gated\
  \ (contact API team; sandbox then production credentials)\n  self_serve: false\nschemes:\n- name: OAuth2\n  type: oauth2\n  description: >-\n    OAuth 2.0 token-based authentication documented for the Axos API Store.\n    Flow details, authorization/token URLs, and scopes are provisioned to\n    onboarded partners and are not published publicly.\n  documented_flow: clientCredentials\n  source: https://www.axosbank.com/developer\n- name: DeveloperDashboardKey\n  type: apiKey\n  in: dashboard-issued\n  description: >-\n    API keys issued to each onboarded developer through a per-user secure\n    developer dashboard, used alongside OAuth 2.0 tokens.\n  source: https://www.axosbank.com/developer\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/axos-bank/refs/heads/main/authentication/axos-bank-authentication.yml
summary_line: oauth2/apiKey · 2 schemes
tags:
- Financial-Services
- Banking
- United States
- Banking-as-a-Service
- Open Finance
- Payments
- Digital Bank
---
