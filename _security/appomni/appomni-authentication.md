---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: appomni-policies-api-openapi.yml
  format: yaml
  label: AppOmni Policies API
  slug: appomni-policies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/appomni/refs/heads/main/openapi/appomni-policies-api-openapi.yml
- filename: appomni-monitored-services-api-openapi.yml
  format: yaml
  label: AppOmni Monitored Services API
  slug: appomni-monitored-services-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/appomni/refs/heads/main/openapi/appomni-monitored-services-api-openapi.yml
- filename: appomni-identity-api-openapi.yml
  format: yaml
  label: AppOmni Identity and Access API
  slug: appomni-identity-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/appomni/refs/heads/main/openapi/appomni-identity-api-openapi.yml
- filename: appomni-agentguard-api-openapi.yml
  format: yaml
  label: AppOmni Agent Guard API
  slug: appomni-agentguard-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/appomni/refs/heads/main/openapi/appomni-agentguard-api-openapi.yml
- filename: appomni-ao-developer-platform-api-openapi.yml
  format: yaml
  label: AppOmni AO Developer Platform API
  slug: appomni-ao-developer-platform-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/appomni/refs/heads/main/openapi/appomni-ao-developer-platform-api-openapi.yml
- filename: appomni-audit-logs-api-openapi.yml
  format: yaml
  label: AppOmni Audit Logs API
  slug: appomni-audit-logs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/appomni/refs/heads/main/openapi/appomni-audit-logs-api-openapi.yml
- filename: appomni-authorization-tokens-api-openapi.yml
  format: yaml
  label: AppOmni Authorization Tokens API
  slug: appomni-authorization-tokens-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/appomni/refs/heads/main/openapi/appomni-authorization-tokens-api-openapi.yml
- filename: appomni-beta-policy-assessment-stats-api-openapi.yml
  format: yaml
  label: AppOmni [Beta] Policy Assessment Stats API
  slug: appomni-beta-policy-assessment-stats-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/appomni/refs/heads/main/openapi/appomni-beta-policy-assessment-stats-api-openapi.yml
- filename: appomni-custom-field-values-for-a-monitored-service-api-openapi.yml
  format: yaml
  label: AppOmni Custom Field Values for a Monitored Service API
  slug: appomni-custom-field-values-for-a-monitored-service-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/appomni/refs/heads/main/openapi/appomni-custom-field-values-for-a-monitored-service-api-openapi.yml
- filename: appomni-custom-fields-api-openapi.yml
  format: yaml
  label: AppOmni Custom Fields API
  slug: appomni-custom-fields-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/appomni/refs/heads/main/openapi/appomni-custom-fields-api-openapi.yml
- filename: appomni-discovery-api-openapi.yml
  format: yaml
  label: AppOmni Discovery API
  slug: appomni-discovery-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/appomni/refs/heads/main/openapi/appomni-discovery-api-openapi.yml
- filename: appomni-insights-api-openapi.yml
  format: yaml
  label: AppOmni Insights API
  slug: appomni-insights-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/appomni/refs/heads/main/openapi/appomni-insights-api-openapi.yml
- filename: appomni-marlin-ai-api-openapi.yml
  format: yaml
  label: AppOmni Marlin AI API
  slug: appomni-marlin-ai-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/appomni/refs/heads/main/openapi/appomni-marlin-ai-api-openapi.yml
- filename: appomni-posture-findings-api-openapi.yml
  format: yaml
  label: AppOmni Posture Findings API
  slug: appomni-posture-findings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/appomni/refs/heads/main/openapi/appomni-posture-findings-api-openapi.yml
- filename: appomni-reports-api-openapi.yml
  format: yaml
  label: AppOmni Reports API
  slug: appomni-reports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/appomni/refs/heads/main/openapi/appomni-reports-api-openapi.yml
- filename: appomni-scim-user-management-api-openapi.yml
  format: yaml
  label: AppOmni SCIM User Management API
  slug: appomni-scim-user-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/appomni/refs/heads/main/openapi/appomni-scim-user-management-api-openapi.yml
- filename: appomni-users-and-roles-api-openapi.yml
  format: yaml
  label: AppOmni Users and Roles API
  slug: appomni-users-and-roles-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/appomni/refs/heads/main/openapi/appomni-users-and-roles-api-openapi.yml
- filename: appomni-valuelist-api-openapi.yml
  format: yaml
  label: AppOmni Value List API
  slug: appomni-valuelist-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/appomni/refs/heads/main/openapi/appomni-valuelist-api-openapi.yml
auth_types:
- http
- apiKey
- oauth2
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Appomni Authentication
name_suffix: Authentication
oauth_flows: []
overview: AppOmni secures its APIs with http, apiKey, and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: AppOmni
provider_slug: appomni
scheme_count: 2
schemes:
- description: 'AppOmni API access token. Created and managed in the AppOmni platform under Settings > API Settings, then sent as `Authorization: Bearer <token>`. All 144 requests in AppOmni''s public Postman collection use this scheme.'
  name: bearerAuth
  obtain: AppOmni platform UI, Settings > API Settings
  parameter: Authorization
  scheme: bearer
  sources:
  - openapi/appomni-security-events-api-openapi.yml
  - openapi/appomni-policies-api-openapi.yml
  - openapi/appomni-compliance-api-openapi.yml
  - openapi/appomni-monitored-services-api-openapi.yml
  - openapi/appomni-identity-api-openapi.yml
  - openapi/appomni-scim-api-openapi.yml
  - openapi/appomni-discovery-insights-api-openapi.yml
  - openapi/appomni-developer-platform-api-openapi.yml
  - openapi/appomni-ai-api-openapi.yml
  type: http
- description: AppOmni-issued ingest token, a different credential from the platform bearer token. Used by AgentGuard (POST /api/v1/ai/prompts/agents/classify) and by the AppOmni Developer Platform ingest endpoint (POST /platform/ingest/v2/ingest/). Retrieved with getIngestToken and rotated with rotateIngestToken on the monitored service it belongs to.
  in: header
  name: ingestToken
  obtain: GET /api/v1/core/monitoredservice/{ms_id}/get_ingest_token/
  parameter: X-AppOmni-Ingest-Token
  rotate: PATCH /api/v1/core/monitoredservice/{ms_id}/rotate_ingest_token/
  sources:
  - openapi/appomni-ai-api-openapi.yml
  - openapi/appomni-developer-platform-api-openapi.yml
  - https://github.com/appomni/n8n-nodes-agentguard/blob/master/credentials/AgentGuardApi.credentials.ts
  type: apiKey
slug: appomni-authentication
source_filename: appomni-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-04'\nmethod: searched\nsource: https://api.appomni.com/ (AppOmni public Postman collection and its per-route documentation)\ndocs: https://api.appomni.com/\nsummary:\n  types:\n    - http\n    - apiKey\n    - oauth2\n  api_key_in:\n    - header\n  primary: Bearer access token issued by the AppOmni platform\n  tenancy: >-\n    Every credential is scoped to one AppOmni tenant. The API host is the customer's own subdomain —\n    https://{instance}.appomni.com — so there is no shared multi-tenant API host to authenticate against.\nschemes:\n  - name: bearerAuth\n    type: http\n    scheme: bearer\n    parameter: Authorization\n    description: >-\n      AppOmni API access token. Created and managed in the AppOmni platform under Settings > API\n      Settings, then sent as `Authorization: Bearer <token>`. All 144 requests in AppOmni's public\n      Postman collection use this scheme.\n    obtain: AppOmni platform UI, Settings > API Settings\n    sources:\n  \
  \    - openapi/appomni-security-events-api-openapi.yml\n      - openapi/appomni-policies-api-openapi.yml\n      - openapi/appomni-compliance-api-openapi.yml\n      - openapi/appomni-monitored-services-api-openapi.yml\n      - openapi/appomni-identity-api-openapi.yml\n      - openapi/appomni-scim-api-openapi.yml\n      - openapi/appomni-discovery-insights-api-openapi.yml\n      - openapi/appomni-developer-platform-api-openapi.yml\n      - openapi/appomni-ai-api-openapi.yml\n  - name: ingestToken\n    type: apiKey\n    in: header\n    parameter: X-AppOmni-Ingest-Token\n    description: >-\n      AppOmni-issued ingest token, a different credential from the platform bearer token. Used by\n      AgentGuard (POST /api/v1/ai/prompts/agents/classify) and by the AppOmni Developer Platform ingest\n      endpoint (POST /platform/ingest/v2/ingest/). Retrieved with getIngestToken and rotated with\n      rotateIngestToken on the monitored service it belongs to.\n    obtain: GET /api/v1/core/monitoredservice/{ms_id}/get_ingest_token/\n\
  \    rotate: PATCH /api/v1/core/monitoredservice/{ms_id}/rotate_ingest_token/\n    sources:\n      - openapi/appomni-ai-api-openapi.yml\n      - openapi/appomni-developer-platform-api-openapi.yml\n      - https://github.com/appomni/n8n-nodes-agentguard/blob/master/credentials/AgentGuardApi.credentials.ts\noauth2:\n  supported: true\n  application_object: AppOmni API Application (OAuthApplication)\n  grants:\n    - refresh_token\n  endpoints:\n    token: POST /oauth/token/\n    introspection: GET /oauth/introspect/\n    revocation: POST /oauth/revoke/\n  standards:\n    - RFC 6749 Refresh Token Grant\n    - RFC 7662 Token Introspection\n    - RFC 7009 Token Revocation\n  parameters:\n    - grant_type (must be \"refresh_token\")\n    - refresh_token\n    - client_id\n    - client_secret\n  scopes_published: false\n  scopes_note: >-\n    AppOmni publishes no OAuth scope reference and no scope parameter appears on the token endpoint.\n    Authorization is enforced by the AppOmni role/permission\
  \ model on the granting user, not by token\n    scopes — the API exposes a per-object permission probe returning\n    {\"permissions\": {\"list\", \"create\", \"update\", \"partial_update\", \"delete\"}}. No scopes/ artifact is\n    emitted because there is nothing published to record.\n  long_lived_tokens: >-\n    POST /api/v1/core/oauthaccesstoken/manual/ grants an access token with a caller-specified\n    expiration date, for service-to-service integrations that cannot run the refresh-token flow.\n  secret_rotation: POST /api/v1/core/oauthapplication/{app_id}/rotate_client_secret/\n  discovery:\n    well_known: false\n    note: >-\n      No /.well-known/oauth-authorization-server or /.well-known/openid-configuration is served on any\n      AppOmni host — see well-known/appomni-well-known.yml. The OAuth endpoints are documented only in\n      the Postman collection.\nmfa_sso:\n  scim: >-\n    Identity-provider integration is via SCIM 2.0 at /scim/v2/ — see openapi/appomni-scim-api-openapi.yml.\n\
  \  breakglass: >-\n    PUT /api/v1/core/user/{user_id}/enable_breakglass and .../disable_breakglass toggle emergency access.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/appomni/refs/heads/main/authentication/appomni-authentication.yml
summary_line: http/apiKey/oauth2 · 2 schemes
tags:
- SaaS Security
- SSPM
- Compliance
- Threat Detection
- CASB
- Zero Trust
- Identity
- SCIM
- AI Security
- Posture Management
---
