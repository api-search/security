---
api_key_in: []
api_specs:
- filename: google-marketing-platform-v1alpha-api-openapi.yml
  format: yaml
  label: Google Marketing Platform Admin V1alpha API
  slug: google-marketing-platform-v1alpha-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/google-marketing-platform/refs/heads/main/openapi/google-marketing-platform-v1alpha-api-openapi.yml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Google Marketing Platform Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Google Marketing Platform Admin secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Google Marketing Platform Admin
provider_slug: google-marketing-platform
scheme_count: 1
schemes:
- canonical_scopes_source: grpc/google-marketing-platform-service-config.yaml
  flows:
  - authorizationUrl: https://accounts.google.com/o/oauth2/auth
    flow: authorizationCode
    scopes: 2
    tokenUrl: https://oauth2.googleapis.com/token
  name: oauth2
  sources:
  - openapi/google-marketing-platform-v1alpha-api-openapi.yml
  - openapi/google-marketing-platform-v1alpha-discovery.json
  type: oauth2
slug: google-marketing-platform-authentication
source_filename: google-marketing-platform-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: searched\nsource: openapi/google-marketing-platform-v1alpha-api-openapi.yml\ndocs: https://developers.google.com/marketing-platform/devguides/api/admin/v1/quickstart\nalso_source:\n  - openapi/google-marketing-platform-v1alpha-discovery.json\n  - grpc/google-marketing-platform-service-config.yaml\n  - well-known/google-marketing-platform-openid-configuration.json\nnote: >-\n  Upgraded from the derived pass with the provider's quickstart and the\n  first-party service config. The derived file captured the oauth2 scheme\n  correctly but missed the two things that actually break a first call: the\n  mandatory Cloud quota project, and the fact that scope failures and quota\n  failures share HTTP 403.\nsummary:\n  types: [oauth2]\n  api_key_supported: false\n  api_key_in: []\n  oauth2_flows: [authorizationCode]\n  application_default_credentials: true\n  mutual_tls: false\n  service_accounts: supported\nschemes:\n  - name: oauth2\n    type: oauth2\n\
  \    flows:\n      - flow: authorizationCode\n        authorizationUrl: https://accounts.google.com/o/oauth2/auth\n        tokenUrl: https://oauth2.googleapis.com/token\n        scopes: 2\n    sources:\n      - openapi/google-marketing-platform-v1alpha-api-openapi.yml\n      - openapi/google-marketing-platform-v1alpha-discovery.json\n    canonical_scopes_source: grpc/google-marketing-platform-service-config.yaml\nauthorization_server:\n  issuer: https://accounts.google.com\n  discovery: https://accounts.google.com/.well-known/openid-configuration\n  discovery_status: 200\n  discovery_checked: '2026-08-13'\n  authorization_endpoint: https://accounts.google.com/o/oauth2/v2/auth\n  token_endpoint: https://oauth2.googleapis.com/token\n  saved_copy: well-known/google-marketing-platform-openid-configuration.json\n  note: >-\n    The API host itself serves no /.well-known/openid-configuration or\n    /.well-known/oauth-authorization-server (both 404). Discovery lives on\n    accounts.google.com,\
  \ the shared Google authorization server.\ncredentials:\n  - kind: oauth-user\n    description: >-\n      Three-legged OAuth as a user who has access to the GMP organization. This\n      is the path the quickstart takes.\n    header: 'Authorization: Bearer <access_token>'\n  - kind: application-default-credentials\n    description: >-\n      Local ADC via gcloud. The quickstart's exact command:\n      gcloud auth application-default login\n      --scopes=\"https://www.googleapis.com/auth/cloud-platform,https://www.googleapis.com/auth/marketingplatformadmin.analytics.read\"\n    header: 'Authorization: Bearer $(gcloud auth application-default print-access-token)'\n  - kind: service-account\n    description: >-\n      Supported through the standard Google auth libraries the GAPIC clients\n      depend on. The service account must itself be granted access to the GMP\n      organization; the API documents no domain-wide-delegation path of its own.\napi_key: false\napi_key_note: >-\n  This\
  \ API accepts no API key for authentication. The Discovery Document\n  declares the standard `key` system parameter on every method, but that is\n  Google's project-identification parameter and does not authenticate a call\n  to this service.\nrequired_setup:\n  - step: Enable the API\n    detail: >-\n      marketingplatformadmin.googleapis.com must be enabled on the calling\n      Google Cloud project.\n  - step: Set a quota project\n    detail: >-\n      \"The Google Marketing Platform Admin API requires a quota project, which\n      is not set by default.\" Without it, correctly scoped credentials still\n      fail. This is the most common first-call failure on this API.\n    source: https://developers.google.com/marketing-platform/devguides/api/admin/v1/quickstart\n  - step: Grant organization access\n    detail: >-\n      The authenticated principal must have access to the target GMP\n      organization; scopes alone do not grant it.\nscopes_detail: scopes/google-marketing-platform-scopes.yml\n\
  failure_modes:\n  - status: 401\n    grpc_status: UNAUTHENTICATED\n    cause: Missing, expired or malformed access token.\n  - status: 403\n    grpc_status: PERMISSION_DENIED\n    cause: >-\n      Wrong scope, no access to the organization, API not enabled, or no quota\n      project set.\n  - status: 403\n    grpc_status: RESOURCE_EXHAUSTED\n    reason: rateLimitExceeded\n    cause: >-\n      Quota, NOT authentication. Shares the 403 status with the genuine auth\n      failures above — branch on error.errors[].reason before deciding a\n      credential is bad.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/google-marketing-platform/refs/heads/main/authentication/google-marketing-platform-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Analytics
- Google Marketing Platform
- Marketing
- Organization Management
- Platform Administration
---
