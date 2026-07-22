---
api_key_in: []
auth_types:
- oauth2
- openIdConnect
- http
description: ''
kind: authentication
layout: security
method: searched
name: Zus Health Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: Zus Health secures its APIs with oauth2, openIdConnect, and http across 4 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: Zus Health
provider_slug: zus-health
scheme_count: 4
schemes:
- description: Machine-to-machine App Client for backend services (no human in the loop). An App Client is issued a clientId and clientSecret used to obtain a bearer access token. Client secret can be rotated via the Auth Service API.
  docs: https://docs.zushealth.com/docs/m2m-application-setup
  flow: clientCredentials
  name: m2m-client-credentials
  rate_limit: 200 token requests per hour per App Client (429 on exceed)
  token_ttl_seconds: 3600
  type: oauth2
- description: Exchange an OIDC-compliant ID token from the customer's own identity provider for a Zus access token, so an application's end users are not required to log in to Zus twice.
  docs: https://docs.zushealth.com/reference/exchange-token-1
  name: token-exchange
  type: openIdConnect
- description: Interactive user sign-in (username + password). MFA is required for all Zus accounts and re-verified every 24 hours. Not subject to the M2M token rate limit.
  docs: https://docs.zushealth.com/docs/user-authentication
  name: user-authentication
  scheme: bearer
  sso_providers:
  - AWS Cognito
  - Google Workspace
  - Microsoft Azure Active Directory
  - Okta
  type: http
- description: Zushooks (outbound webhooks) support Basic (username/password) or OAuth client-credentials authentication against the customer's receiving endpoint (webhookUrl, clientId, clientSecret, tokenUrl, audience).
  docs: https://docs.zushealth.com/docs/zushooks
  name: webhook-auth
  scheme: basic
  type: http
slug: zus-health-authentication
source_filename: zus-health-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://docs.zushealth.com/docs/user-authentication\ndocs: https://docs.zushealth.com/docs/user-authentication\nsummary:\n  types: [oauth2, openIdConnect, http]\n  oauth2_flows: [clientCredentials]\n  http_schemes: [bearer, basic]\n  standard: OAuth 2.0\n  mfa_required: true\nnotes: >-\n  Zus secures all API access with OAuth 2.0. Every API request must carry a Bearer access token.\n  Access tokens are valid for 1 hour. Both the FHIR REST API (api.zusapi.com) and the GraphQL FQS\n  API (fqs.zusapi.com) accept the same bearer token.\nschemes:\n- name: m2m-client-credentials\n  type: oauth2\n  flow: clientCredentials\n  description: >-\n    Machine-to-machine App Client for backend services (no human in the loop). An App Client is\n    issued a clientId and clientSecret used to obtain a bearer access token. Client secret can be\n    rotated via the Auth Service API.\n  token_ttl_seconds: 3600\n  rate_limit: 200 token requests\
  \ per hour per App Client (429 on exceed)\n  docs: https://docs.zushealth.com/docs/m2m-application-setup\n- name: token-exchange\n  type: openIdConnect\n  description: >-\n    Exchange an OIDC-compliant ID token from the customer's own identity provider for a Zus access\n    token, so an application's end users are not required to log in to Zus twice.\n  docs: https://docs.zushealth.com/reference/exchange-token-1\n- name: user-authentication\n  type: http\n  scheme: bearer\n  description: >-\n    Interactive user sign-in (username + password). MFA is required for all Zus accounts and\n    re-verified every 24 hours. Not subject to the M2M token rate limit.\n  sso_providers: [AWS Cognito, Google Workspace, Microsoft Azure Active Directory, Okta]\n  docs: https://docs.zushealth.com/docs/user-authentication\n- name: webhook-auth\n  type: http\n  scheme: basic\n  description: >-\n    Zushooks (outbound webhooks) support Basic (username/password) or OAuth client-credentials\n    authentication\
  \ against the customer's receiving endpoint (webhookUrl, clientId, clientSecret,\n    tokenUrl, audience).\n  docs: https://docs.zushealth.com/docs/zushooks\nauthorization_model:\n  style: role-based\n  docs: https://docs.zushealth.com/docs/roles-and-permissions\n  note: >-\n    Access is governed by roles and permissions plus data-access scoping (data you created, or a\n    patient your organization has a treatment relationship with) rather than OAuth scope strings;\n    no public OAuth scope reference is published, so no scopes/ artifact is emitted.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/zus-health/refs/heads/main/authentication/zus-health-authentication.yml
summary_line: oauth2/openIdConnect/http · 4 schemes
tags:
- Company
- Health
- Healthcare
- FHIR
- Interoperability
- Health Data
- Patient Records
- EHR
- GraphQL
- Webhooks
---
