---
anonymous_access: false
api_key_in:
- cookie
api_specs:
- filename: airmdr-case-manager-openapi.yml
  format: yaml
  label: AirMDR Case Manager API
  slug: airmdr-case-manager-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/airmdr/refs/heads/main/openapi/airmdr-case-manager-openapi.yml
- filename: airmdr-user-management-service-openapi.yml
  format: yaml
  label: AirMDR User Management Service API
  slug: airmdr-user-management-service-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/airmdr/refs/heads/main/openapi/airmdr-user-management-service-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Airmdr Authentication
name_suffix: Authentication
oauth_flows: []
overview: AirMDR secures its APIs with apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: AirMDR
provider_slug: airmdr
scheme_count: 2
schemes:
- in: cookie
  name: SessionCookie
  parameter: Session
  sources:
  - openapi/airmdr-case-manager-openapi.yml
  - openapi/airmdr-user-management-service-openapi.yml
  token_lifecycle:
    expiry: tokens can expire; docs advise handling 401 Unauthorized by checking for token expiration and prefer "scoped and expiring tokens" (no scope vocabulary is published)
    issued_by: Admin dashboard → API Tokens → Create API Token (Admin or Super Admin role required); also createAPITokenForUserAPI (POST /users/tokens) and createAPITokenForSlackWorkflowAPI
    listing: listTokensForUserAPI (GET /users/tokens)
    revocation: delete the token in the dashboard or deleteTokenAPI (DELETE /users/tokens/{token_id})
    shown_once: true
  type: apiKey
  usage: 'curl --location https://app.airmdr.com/airmdrapi/organization --header ''Cookie: Session="<API Token Here>"'''
- in: path
  name: WebhookURLSecret
  note: not a securityScheme in the spec; documented in the operation description and the M28.1 release notes
  operation: createAlertFromWebhookAPI (POST /webhooks/{webhook_id}/{secret}/alerts)
  parameter: '{webhook_id}/{secret}'
  sources:
  - openapi/airmdr-case-manager-openapi.yml
  type: url-path-secret
  usage: authenticated purely by webhook_id + secret embedded in the URL path; 404 on unknown id or invalid secret
slug: airmdr-authentication
source_filename: airmdr-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-19'\nmethod: searched\nsource: openapi/airmdr-case-manager-openapi.yml, openapi/airmdr-user-management-service-openapi.yml\ndocs: https://docs.airmdr.com/api-reference/apitoken\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - cookie\n  oauth2: false\n  oidc: false\nschemes:\n- name: SessionCookie\n  type: apiKey\n  in: cookie\n  parameter: Session\n  usage: 'curl --location https://app.airmdr.com/airmdrapi/organization --header ''Cookie: Session=\"<API Token Here>\"'''\n  token_lifecycle:\n    issued_by: Admin dashboard → API Tokens → Create API Token (Admin or Super Admin role required); also createAPITokenForUserAPI (POST /users/tokens) and createAPITokenForSlackWorkflowAPI\n    shown_once: true\n    listing: listTokensForUserAPI (GET /users/tokens)\n    revocation: delete the token in the dashboard or deleteTokenAPI (DELETE /users/tokens/{token_id})\n    expiry: tokens can expire; docs advise handling 401 Unauthorized by checking for token expiration\
  \ and prefer \"scoped and expiring tokens\" (no scope vocabulary is published)\n  sources:\n  - openapi/airmdr-case-manager-openapi.yml\n  - openapi/airmdr-user-management-service-openapi.yml\n- name: WebhookURLSecret\n  type: url-path-secret\n  in: path\n  parameter: '{webhook_id}/{secret}'\n  operation: createAlertFromWebhookAPI (POST /webhooks/{webhook_id}/{secret}/alerts)\n  usage: authenticated purely by webhook_id + secret embedded in the URL path; 404 on unknown id or invalid secret\n  sources:\n  - openapi/airmdr-case-manager-openapi.yml\n  note: not a securityScheme in the spec; documented in the operation description and the M28.1 release notes\ncontext_headers:\n  required: [User-ID, Organization-ID]\n  optional: [X-Request-ID, Execution-ID, Organization-Hosturl]\n  note: the docs say these are \"automatically preloaded\" into request examples when a token is generated\nconsole_sso:\n  providers: [Azure AD, Google, Okta]\n  docs: https://docs.airmdr.com/essentials/SSO-Overview\n\
  \  note: console user sign-in only; not an API authentication surface\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/airmdr/refs/heads/main/authentication/airmdr-authentication.yml
summary_line: apiKey · 2 schemes
tags:
- Security
- Managed Detection and Response
- Security Operations
- Alert Triage
- Incident Response
- AI Agents
- SOC Automation
- Threat Detection
- MCP
- A2A
---
