---
api_key_in: []
api_specs:
- filename: timescale-analytics-api-openapi.yml
  format: yaml
  label: Timescale Analytics API
  slug: timescale-analytics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/timescale/refs/heads/main/openapi/timescale-analytics-api-openapi.yml
- filename: timescale-auth-api-openapi.yml
  format: yaml
  label: Timescale Auth API
  slug: timescale-auth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/timescale/refs/heads/main/openapi/timescale-auth-api-openapi.yml
- filename: timescale-feedback-api-openapi.yml
  format: yaml
  label: Timescale Feedback API
  slug: timescale-feedback-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/timescale/refs/heads/main/openapi/timescale-feedback-api-openapi.yml
- filename: timescale-health-api-openapi.yml
  format: yaml
  label: Timescale Health API
  slug: timescale-health-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/timescale/refs/heads/main/openapi/timescale-health-api-openapi.yml
- filename: timescale-invites-api-openapi.yml
  format: yaml
  label: Timescale Invites API
  slug: timescale-invites-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/timescale/refs/heads/main/openapi/timescale-invites-api-openapi.yml
- filename: timescale-pricing-api-openapi.yml
  format: yaml
  label: Timescale Pricing API
  slug: timescale-pricing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/timescale/refs/heads/main/openapi/timescale-pricing-api-openapi.yml
- filename: timescale-projects-api-openapi.yml
  format: yaml
  label: Timescale Projects API
  slug: timescale-projects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/timescale/refs/heads/main/openapi/timescale-projects-api-openapi.yml
- filename: timescale-read-replica-sets-api-openapi.yml
  format: yaml
  label: Timescale Read Replica Sets API
  slug: timescale-read-replica-sets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/timescale/refs/heads/main/openapi/timescale-read-replica-sets-api-openapi.yml
- filename: timescale-services-api-openapi.yml
  format: yaml
  label: Timescale Services API
  slug: timescale-services-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/timescale/refs/heads/main/openapi/timescale-services-api-openapi.yml
- filename: timescale-spaces-api-openapi.yml
  format: yaml
  label: Timescale Spaces API
  slug: timescale-spaces-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/timescale/refs/heads/main/openapi/timescale-spaces-api-openapi.yml
- filename: timescale-vpcs-api-openapi.yml
  format: yaml
  label: Timescale VP Cs API
  slug: timescale-vpcs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/timescale/refs/heads/main/openapi/timescale-vpcs-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: searched
name: Timescale Authentication
name_suffix: Authentication
oauth_flows: []
overview: Timescale secures its APIs with http across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Timescale
provider_slug: timescale
scheme_count: 3
schemes:
- api: Tiger Cloud API
  description: 'HTTP Basic authentication with Tiger Cloud client credentials: the public access key as the username and the secret key as the password. The docs publish the environment-variable names TIGERDATA_PROJECT_ID, TIGERDATA_ACCESS_KEY and TIGERDATA_SECRET_KEY and the request form `curl -u "${TIGERDATA_ACCESS_KEY}:${TIGERDATA_SECRET_KEY}"`. Credentials are created in Tiger Console; the secret key is displayed once and cannot be retrieved again.'
  name: basicAuth
  scheme: basic
  sources:
  - https://www.tigerdata.com/docs/get-started/quickstart/rest-api
  spec_declared: false
  type: http
- api: Tiger Cloud API
  description: OAuth user bearer token, used by Tiger Console and by the Tiger CLI after `tiger auth login`. The getAuthInfo (GET /auth/info) response discriminates the two credential shapes with a `type` field whose enum is ["apiKey", "oauth"] — `apiKey` for personal-access-token callers, `oauth` for OAuth user callers. The logout operation revokes the caller's refresh token server-side and applies only to OAuth bearer callers.
  name: bearerAuth (Tiger Cloud OAuth)
  scheme: bearer
  sources:
  - openapi/timescale-tiger-cloud-openapi-original.yml
  spec_declared: false
  type: http
- api: Ghost API
  applied: 'document-level security: [{BearerAuth: []}]; only GET /health opts out with security: []'
  description: 'User JWT or API key token (e.g. `gt_...`) sent as `Authorization: Bearer <token>`.'
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/timescale-ghost-openapi-original.yml
  spec_declared: true
  type: http
slug: timescale-authentication
source_filename: timescale-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-05'\nmethod: searched\nsource: openapi/timescale-ghost-openapi-original.yml\ndocs: https://www.tigerdata.com/docs/get-started/quickstart/rest-api\ndocs_credentials: https://www.tigerdata.com/docs/use-timescale/latest/security/client-credentials\nsummary:\n  types: [http]\n  http_schemes: [basic, bearer]\n  api_key_in: []\n  oauth2_flows: []\n  note: >-\n    The Tiger Cloud OpenAPI declares NO securitySchemes block at all — auth is\n    described only in prose in the operation descriptions and in the docs. The schemes\n    below were upgraded from derived to searched using the published quickstart, which\n    shows the exact credential form. Only the Ghost spec declares a scheme natively.\nschemes:\n- name: basicAuth\n  type: http\n  scheme: basic\n  api: Tiger Cloud API\n  description: >-\n    HTTP Basic authentication with Tiger Cloud client credentials: the public access\n    key as the username and the secret key as the password. The docs publish the\n\
  \    environment-variable names TIGERDATA_PROJECT_ID, TIGERDATA_ACCESS_KEY and\n    TIGERDATA_SECRET_KEY and the request form\n    `curl -u \"${TIGERDATA_ACCESS_KEY}:${TIGERDATA_SECRET_KEY}\"`. Credentials are\n    created in Tiger Console; the secret key is displayed once and cannot be\n    retrieved again.\n  sources: [https://www.tigerdata.com/docs/get-started/quickstart/rest-api]\n  spec_declared: false\n- name: bearerAuth (Tiger Cloud OAuth)\n  type: http\n  scheme: bearer\n  api: Tiger Cloud API\n  description: >-\n    OAuth user bearer token, used by Tiger Console and by the Tiger CLI after\n    `tiger auth login`. The getAuthInfo (GET /auth/info) response discriminates the\n    two credential shapes with a `type` field whose enum is [\"apiKey\", \"oauth\"] —\n    `apiKey` for personal-access-token callers, `oauth` for OAuth user callers. The\n    logout operation revokes the caller's refresh token server-side and applies only\n    to OAuth bearer callers.\n  sources: [openapi/timescale-tiger-cloud-openapi-original.yml]\n\
  \  spec_declared: false\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  api: Ghost API\n  description: 'User JWT or API key token (e.g. `gt_...`) sent as `Authorization: Bearer <token>`.'\n  sources: [openapi/timescale-ghost-openapi-original.yml]\n  spec_declared: true\n  applied: 'document-level security: [{BearerAuth: []}]; only GET /health opts out with security: []'\nkey_management:\n  tiger_cloud:\n    where: Tiger Console → client credentials\n    scoping: a personal access token is scoped to a single project; getProjects returns\n      only that project for PAT callers, all projects for OAuth callers\n    rotation: secret key shown once at creation, not retrievable afterwards\n  ghost:\n    where: 'POST /spaces/{space_id}/api_keys (createApiKey)'\n    prefix: gt_\n    scoping: per space\n    revocation: 'DELETE /spaces/{space_id}/api_keys/{prefix} (deleteApiKey) — keys are\n      addressed by prefix, not by full value'\nmfa_sso:\n  mfa: available; Scale and Enterprise projects\
  \ can require MFA or SSO for every project\n    member (changelog entry dated 2026-07-23)\n  sso_saml: Enterprise plan\n  source: https://www.tigerdata.com/security\noauth_scopes: none published — no OAuth2 securityScheme and no scope reference page;\n  scopes/ is intentionally absent\ngaps:\n- The Tiger Cloud spec omits securitySchemes entirely, so any generated client or agent\n  must read prose to authenticate.\n- Neither spec documents token lifetime, refresh, or rate limits.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/timescale/refs/heads/main/authentication/timescale-authentication.yml
summary_line: http · 3 schemes
tags:
- Company
- Database
- PostgreSQL
- Time Series
- Analytics
- Cloud Infrastructure
- Data Platform
- Vector Search
- Developer Tools
- Open Source
---
