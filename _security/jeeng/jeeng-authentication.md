---
api_key_in: []
api_specs:
- filename: jeeng-advertisers-openapi.yml
  format: yaml
  label: Jeeng Email Monetization — Advertisers API
  slug: jeeng-email-monetization-advertisers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jeeng/refs/heads/main/openapi/jeeng-advertisers-openapi.yml
- filename: jeeng-publishers-openapi.yml
  format: yaml
  label: Jeeng Email Monetization — Publishers API
  slug: jeeng-email-monetization-publishers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jeeng/refs/heads/main/openapi/jeeng-publishers-openapi.yml
- filename: jeeng-authentication-openapi.yml
  format: yaml
  label: Jeeng Email Monetization — Authentication
  slug: jeeng-email-monetization-authentication
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jeeng/refs/heads/main/openapi/jeeng-authentication-openapi.yml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Jeeng Authentication
name_suffix: Authentication
oauth_flows: []
overview: Jeeng secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Jeeng
provider_slug: jeeng
scheme_count: 1
schemes:
- discovery: https://login.microsoftonline.com/revenuestripe.onmicrosoft.com/v2.0/.well-known/openid-configuration
  flows:
  - flow: clientCredentials
    scopes:
      api://revenuestripe.onmicrosoft.com/partners/.default: Grants the permissions for all partner API endpoints — advertiser and publisher reporting, campaigns, creatives, and the performance reports.
    tokenUrl: https://login.microsoftonline.com/revenuestripe.onmicrosoft.com/oauth2/v2.0/token
  identity_provider: Microsoft Entra ID (Azure AD)
  name: sec0
  sources:
  - openapi/jeeng-authentication-openapi.yml
  - openapi/jeeng-advertisers-openapi.yml
  - openapi/jeeng-publishers-openapi.yml
  tenant: revenuestripe.onmicrosoft.com
  tenant_id: 0d82cfa7-eb30-4eb7-83e2-574580d8fb08
  type: oauth2
slug: jeeng-authentication
source_filename: jeeng-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-12'\nmethod: searched\nsource: https://developers.jeeng.com/reference/getting-an-access-token\ndocs: https://developers.jeeng.com/reference/getting-an-access-token\nsummary:\n  types:\n  - oauth2\n  primary: oauth2\n  flow: client_credentials\n  token_placement: Authorization Bearer header\n  provisioning: sales-gated — client id and client secret are issued by Jeeng technical support / the\n    account manager; there is no self-serve developer signup.\nschemes:\n- name: sec0\n  type: oauth2\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://login.microsoftonline.com/revenuestripe.onmicrosoft.com/oauth2/v2.0/token\n    scopes:\n      api://revenuestripe.onmicrosoft.com/partners/.default: Grants the permissions for all partner\n        API endpoints — advertiser and publisher reporting, campaigns, creatives, and the\n        performance reports.\n  identity_provider: Microsoft Entra ID (Azure AD)\n  tenant: revenuestripe.onmicrosoft.com\n  tenant_id:\
  \ 0d82cfa7-eb30-4eb7-83e2-574580d8fb08\n  discovery: https://login.microsoftonline.com/revenuestripe.onmicrosoft.com/v2.0/.well-known/openid-configuration\n  sources:\n  - openapi/jeeng-authentication-openapi.yml\n  - openapi/jeeng-advertisers-openapi.yml\n  - openapi/jeeng-publishers-openapi.yml\nrequest:\n  method: POST\n  content_type: application/x-www-form-urlencoded\n  required_fields:\n  - client_id\n  - client_secret\n  - grant_type\n  - scope\n  grant_type: client_credentials\n  scope: api://revenuestripe.onmicrosoft.com/partners/.default\nresponse:\n  token_type: Bearer\n  expires_in: 3599\n  fields:\n  - token_type\n  - expires_in\n  - ext_expires_in\n  - access_token\nusage:\n  header: 'Authorization: Bearer <access_token>'\n  applies_to:\n  - https://powerinbox.azure-api.net/\nnotes:\n- >-\n  The OpenAPI securityScheme Jeeng publishes for the advertiser and publisher APIs declares\n  `type: oauth2` with an empty `flows` object; the flow, token URL and scope below are read\
  \ from the\n  provider's own authentication reference page rather than from the spec.\n- 'Documented failure mode: requesting a token with any scope other than the partners scope returns\n  HTTP 401 with the message \"Not authorized to this endpoint.\" — and because a wrong-scope token can\n  still succeed on some endpoints, it often surfaces only on the performance report endpoints.'\n- The tenant discovery document at login.microsoftonline.com was probed anonymously on 2026-08-12\n  (HTTP 200) and confirms the issuer and token endpoint above.\nx-evidence:\n- url: https://developers.jeeng.com/reference/getting-an-access-token.md\n  http_status: 200\n  fetched: '2026-08-12'\n- url: https://login.microsoftonline.com/revenuestripe.onmicrosoft.com/v2.0/.well-known/openid-configuration\n  http_status: 200\n  fetched: '2026-08-12'\n- url: https://powerinbox.azure-api.net/reporting/containers?api-version=1.0\n  http_status: 401\n  fetched: '2026-08-12'\n  note: unauthenticated call returns {\"\
  statusCode\":401,\"message\":\"Unauthorized\"}\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/jeeng/refs/heads/main/authentication/jeeng-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Company
- Advertising
- Publishing
- Email
- Push Notifications
- Monetization
- AdTech
- Newsletters
- Audience Engagement
- Reporting
- Analytics
- OData
- OAuth
---
