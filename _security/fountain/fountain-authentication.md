---
api_key_in:
- header
auth_types:
- oauth2
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Fountain Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: Fountain secures its APIs with oauth2 and apiKey across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: Fountain
provider_slug: fountain
scheme_count: 2
schemes:
- applies_to: https://services.fountain.com/api/
  description: Primary auth for the unified services.fountain.com gateway. Exchange an API key/secret for a bearer token via the client-credentials flow; the token is valid for 60 minutes and is sent as an Authorization bearer header on subsequent requests (e.g. servicehire/v2/applicants, serviceworkforce/workers).
  flows:
  - flow: clientCredentials
    tokenUrl: https://services.fountain.com/api/servicesecurity/processes/apikey/oauth/token
    token_ttl_seconds: 3600
  name: OAuth2ClientCredentials
  type: oauth2
- applies_to:
  - https://api.fountain.com/v2/
  - https://{region}.fountain.com/api/v2
  description: Legacy per-tenant API key model for the classic Hire v2 API on tenant hosts (api.fountain.com/v2 for app.fountain.com / web.fountain.com accounts, or {region}.fountain.com/api/v2 for region-pinned tenants such as us-2). The API key is generated per company under Developer Settings.
  in: header
  name: XAccessToken
  parameter_name: X-ACCESS-TOKEN
  type: apiKey
slug: fountain-authentication
source_filename: fountain-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: https://developer.fountain.com/reference/overview\ndocs: https://developer.fountain.com/reference/overview\nsummary:\n  types: [oauth2, apiKey]\n  api_key_in: [header]\n  oauth2_flows: [clientCredentials]\nschemes:\n- name: OAuth2ClientCredentials\n  type: oauth2\n  description: >-\n    Primary auth for the unified services.fountain.com gateway. Exchange an API\n    key/secret for a bearer token via the client-credentials flow; the token is\n    valid for 60 minutes and is sent as an Authorization bearer header on\n    subsequent requests (e.g. servicehire/v2/applicants, serviceworkforce/workers).\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://services.fountain.com/api/servicesecurity/processes/apikey/oauth/token\n    token_ttl_seconds: 3600\n  applies_to: https://services.fountain.com/api/\n- name: XAccessToken\n  type: apiKey\n  in: header\n  parameter_name: X-ACCESS-TOKEN\n  description: >-\n    Legacy per-tenant\
  \ API key model for the classic Hire v2 API on tenant hosts\n    (api.fountain.com/v2 for app.fountain.com / web.fountain.com accounts, or\n    {region}.fountain.com/api/v2 for region-pinned tenants such as us-2). The API\n    key is generated per company under Developer Settings.\n  applies_to:\n  - https://api.fountain.com/v2/\n  - https://{region}.fountain.com/api/v2\nnotes: >-\n  Two coexisting models: OAuth2 client-credentials on the new services gateway and\n  a legacy X-ACCESS-TOKEN header key on tenant hosts. No granular OAuth scope surface\n  is documented (client-credentials tokens carry the account's full permission set),\n  so no scopes/ artifact is emitted.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/fountain/refs/heads/main/authentication/fountain-authentication.yml
summary_line: oauth2/apiKey · 2 schemes
tags:
- Company
- Enterprise
- Hiring
- Recruiting
- Applicant Tracking
- Human Resources
- Workforce Management
- Onboarding
- Scheduling
- HR Tech
- Frontline
---
