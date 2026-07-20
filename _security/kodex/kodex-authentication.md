---
api_key_in:
- header
auth_types:
- apiKey
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Kodex Authentication
name_suffix: Authentication
oauth_flows: []
overview: Kodex secures its APIs with apiKey and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Kodex
provider_slug: kodex
scheme_count: 2
schemes:
- applies_to:
  - Kodex Verification API
  - Kodex Request Portal API
  description: Scoped API keys for service-to-service calls, sent in a request header. Keys are created and managed by organization admins and are provisioned per organization, scoped to what the integration needs.
  in: header
  name: X-API-Key
  parameter_name: X-API-Key
  scoped: true
  sources:
  - https://www.kodexglobal.com/api
  - https://docs.kodexapi.com/request-portal/reference/request-api
  - https://docs.kodexapi.com/verifications/reference/
  type: apiKey
- description: Kodex documents OAuth for user-context flows, described as the same auth posture as the portal. No authorization/token endpoints, flows, or scope reference are published on the public surface, so no flows are recorded here.
  flows: []
  name: OAuth (user-context)
  sources:
  - https://www.kodexglobal.com/api
  type: oauth2
slug: kodex-authentication
source_filename: kodex-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: https://www.kodexglobal.com/api\ndocs: https://docs.kodexapi.com/\nnotes: Kodex publishes no downloadable OpenAPI definition, so this profile is captured\n  from the provider's own published API page and from the API-key configuration declared\n  by the two ReadMe documentation projects (Request Portal and Verifications API).\nsummary:\n  types:\n  - apiKey\n  - oauth2\n  api_key_in:\n  - header\n  oauth2_flows: []\nschemes:\n- name: X-API-Key\n  type: apiKey\n  in: header\n  parameter_name: X-API-Key\n  scoped: true\n  description: Scoped API keys for service-to-service calls, sent in a request header.\n    Keys are created and managed by organization admins and are provisioned per organization,\n    scoped to what the integration needs.\n  applies_to:\n  - Kodex Verification API\n  - Kodex Request Portal API\n  sources:\n  - https://www.kodexglobal.com/api\n  - https://docs.kodexapi.com/request-portal/reference/request-api\n\
  \  - https://docs.kodexapi.com/verifications/reference/\n- name: OAuth (user-context)\n  type: oauth2\n  description: Kodex documents OAuth for user-context flows, described as the same auth\n    posture as the portal. No authorization/token endpoints, flows, or scope reference\n    are published on the public surface, so no flows are recorded here.\n  flows: []\n  sources:\n  - https://www.kodexglobal.com/api\nportal_authentication:\n  sso: true\n  description: Enterprise SSO and centralized access management through the customer's\n    existing identity provider, with automated provisioning, role-based permissions,\n    and granular admin controls.\n  source: https://www.kodexglobal.com/security-compliance\naudit:\n  description: Every API call is logged to the same audit trail as the Kodex application,\n    giving one source of truth across both surfaces.\n  source: https://www.kodexglobal.com/api\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/kodex/refs/heads/main/authentication/kodex-authentication.yml
summary_line: apiKey/oauth2 · 2 schemes
tags:
- Company
- Law Enforcement
- Compliance
- Legal
- Identity Verification
- Government
- Security
- Threat Intelligence
- Data Requests
- Trust and Safety
---
