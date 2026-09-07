---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: aclaimant-platform-api-openapi.json
  format: json
  label: Aclaimant Platform API
  slug: aclaimant-platform-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aclaimant/refs/heads/main/openapi/aclaimant-platform-api-openapi.json
auth_types:
- apiKey
- http-bearer
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Aclaimant Authentication
name_suffix: Authentication
oauth_flows: []
overview: Aclaimant secures its APIs with apiKey and http-bearer across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Aclaimant
provider_slug: aclaimant
scheme_count: 2
schemes:
- api: Aclaimant Platform API
  applied_to: all 25 operations (every operation declares security apiKeyAuth)
  in: header
  key_prefix: not published
  name: apiKeyAuth
  parameter: x-aclaimant-api-key
  provisioning: Not self-serve. There is no developer signup; a key is issued through Aclaimant during implementation. The pricing page lists "Core System Integrations" as a paid add-on on the RMIS Core tier but does not say it is what gates API access.
  rotation: not documented
  sources:
  - openapi/aclaimant-platform-api-openapi.json
  type: apiKey
- api: Aclaimant Partner / Third-party API
  applied_to: both documented endpoints
  header: 'Authorization: Bearer <bearer-token>'
  name: partnerBearer
  provisioning: 'Published verbatim: "Aclaimant will provide you with a bearer token".'
  refresh: not documented
  scheme: bearer
  sources:
  - https://developer.aclaimant.com/partner/index.html
  token_lifetime: not documented
  type: http
slug: aclaimant-authentication
source_filename: aclaimant-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-06'\nmethod: searched\nsource: >-\n  openapi/aclaimant-platform-api-openapi.json, https://developer.aclaimant.com/partner/index.html,\n  https://support.aclaimant.com/hc/en-us/sections/47940330249371-User-Authentication-Single-Sign-On\ndocs: https://developer.aclaimant.com/partner/index.html\nsummary:\n  types:\n  - apiKey\n  - http-bearer\n  api_key_in:\n  - header\n  oauth2: false\n  openid_connect: false\n  mutual_tls: false\nschemes:\n- name: apiKeyAuth\n  api: Aclaimant Platform API\n  type: apiKey\n  in: header\n  parameter: x-aclaimant-api-key\n  applied_to: all 25 operations (every operation declares security apiKeyAuth)\n  key_prefix: not published\n  rotation: not documented\n  provisioning: >-\n    Not self-serve. There is no developer signup; a key is issued through Aclaimant during implementation.\n    The pricing page lists \"Core System Integrations\" as a paid add-on on the RMIS Core tier but does not say\n    it is what gates API access.\n\
  \  sources:\n  - openapi/aclaimant-platform-api-openapi.json\n- name: partnerBearer\n  api: Aclaimant Partner / Third-party API\n  type: http\n  scheme: bearer\n  header: 'Authorization: Bearer <bearer-token>'\n  applied_to: both documented endpoints\n  provisioning: 'Published verbatim: \"Aclaimant will provide you with a bearer token\".'\n  token_lifetime: not documented\n  refresh: not documented\n  sources:\n  - https://developer.aclaimant.com/partner/index.html\nend_user_authentication:\n  scope: web application login only - NOT API authorization\n  methods:\n  - password credentials\n  - SAML 2.0 SSO (Okta, Microsoft Azure AD, Google Workspace)\n  - Azure OAuth 2.0 SSO\n  policy_control: >-\n    Authentication policies can be managed per user\n    (https://support.aclaimant.com/hc/en-us/articles/13653466063771-Managing-Authentication-Policies-by-User).\n  packaging: Single Sign-On (SSO) is a paid add-on on the RMIS Core tier.\n  login_url: https://dashboard.aclaimant.com/login\n\
  \  sources:\n  - https://support.aclaimant.com/hc/en-us/sections/47940330249371-User-Authentication-Single-Sign-On\nscopes:\n  published: false\n  note: >-\n    No OAuth scopes or API permission model is published. Authorization is implicit in the key: a Platform API\n    key acts within the company/collective it is issued for, and requests carry company-ident explicitly. No\n    scopes/ artifact is emitted because there is no scope surface to derive one from.\ngaps:\n- No key prefix, key format or rotation guidance published.\n- No token lifetime or refresh flow for the partner bearer token.\n- No OAuth 2.0 / OIDC authorization for API access (SSO covers human login only).\n- No /.well-known/openid-configuration or oauth-authorization-server on any host (all 404).\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/aclaimant/refs/heads/main/authentication/aclaimant-authentication.yml
summary_line: apiKey/http-bearer · 2 schemes
tags:
- Risk Management
- Insurance
- Claims Management
- Incident Management
- Safety
- RMIS
- Workers Compensation
- OSHA
- Enterprise Risk Management
- Insurtech
---
