---
api_key_in:
- header
api_specs:
- filename: moogsoft-alerts-incidents-openapi.yaml
  format: yaml
  label: Moogsoft Alerts/Incidents API
  slug: alerts-incidents
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/moogsoft/refs/heads/main/openapi/moogsoft-alerts-incidents-openapi.yaml
- filename: moogsoft-azure-service-openapi.yaml
  format: yaml
  label: Moogsoft Azure Application Insights API
  slug: azure-app-insights
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/moogsoft/refs/heads/main/openapi/moogsoft-azure-service-openapi.yaml
- filename: moogsoft-byo-api-service-openapi.yaml
  format: yaml
  label: Moogsoft Create Your Own Integration API
  slug: create-your-own-integration
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/moogsoft/refs/heads/main/openapi/moogsoft-byo-api-service-openapi.yaml
- filename: moogsoft-cloudwatch-service-openapi.yaml
  format: yaml
  label: Moogsoft Amazon CloudWatch API
  slug: cloudwatch
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/moogsoft/refs/heads/main/openapi/moogsoft-cloudwatch-service-openapi.yaml
- filename: moogsoft-collectors-openapi.yaml
  format: yaml
  label: Moogsoft Collector V2 API
  slug: collector
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/moogsoft/refs/heads/main/openapi/moogsoft-collectors-openapi.yaml
- filename: moogsoft-config-openapi.yaml
  format: yaml
  label: Moogsoft Config API
  slug: config
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/moogsoft/refs/heads/main/openapi/moogsoft-config-openapi.yaml
- filename: moogsoft-events-integration-openapi.yaml
  format: yaml
  label: Moogsoft Events Integration API
  slug: events-integration
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/moogsoft/refs/heads/main/openapi/moogsoft-events-integration-openapi.yaml
- filename: moogsoft-incident-responder-openapi.yaml
  format: yaml
  label: Moogsoft On-Call API
  slug: on-call
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/moogsoft/refs/heads/main/openapi/moogsoft-incident-responder-openapi.yaml
- filename: moogsoft-metric-processor-openapi.yaml
  format: yaml
  label: Moogsoft Rollup Service API
  slug: rollup-service
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/moogsoft/refs/heads/main/openapi/moogsoft-metric-processor-openapi.yaml
- filename: moogsoft-metrics-integration-openapi.yaml
  format: yaml
  label: Moogsoft Metrics API
  slug: metrics
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/moogsoft/refs/heads/main/openapi/moogsoft-metrics-integration-openapi.yaml
- filename: moogsoft-pagerduty-service-openapi.yaml
  format: yaml
  label: Moogsoft PagerDuty Integration API
  slug: pagerduty
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/moogsoft/refs/heads/main/openapi/moogsoft-pagerduty-service-openapi.yaml
- filename: moogsoft-probable-rootcause-openapi.yaml
  format: yaml
  label: Moogsoft Probable Root Cause API
  slug: probable-root-cause
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/moogsoft/refs/heads/main/openapi/moogsoft-probable-rootcause-openapi.yaml
- filename: moogsoft-similar-incidents-openapi.yaml
  format: yaml
  label: Moogsoft Similar Incidents API
  slug: similar-incidents
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/moogsoft/refs/heads/main/openapi/moogsoft-similar-incidents-openapi.yaml
- filename: moogsoft-ui-services-openapi.yaml
  format: yaml
  label: Moogsoft UI Services API
  slug: ui-services
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/moogsoft/refs/heads/main/openapi/moogsoft-ui-services-openapi.yaml
- filename: moogsoft-user-management-openapi.yaml
  format: yaml
  label: Moogsoft User Management API
  slug: user-management
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/moogsoft/refs/heads/main/openapi/moogsoft-user-management-openapi.yaml
- filename: moogsoft-webhook-service-v2-openapi.yaml
  format: yaml
  label: Moogsoft Webhook API
  slug: webhook
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/moogsoft/refs/heads/main/openapi/moogsoft-webhook-service-v2-openapi.yaml
- filename: moogsoft-workflow-engine-service-openapi.yaml
  format: yaml
  label: Moogsoft Workflow Engine API
  slug: workflow-engine
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/moogsoft/refs/heads/main/openapi/moogsoft-workflow-engine-service-openapi.yaml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Moogsoft Authentication
name_suffix: Authentication
oauth_flows: []
overview: Moogsoft secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Moogsoft
provider_slug: moogsoft
scheme_count: 1
schemes:
- description: API Key for accessing Alerts/Incidents API
  in: header
  name: ApiKeyAuth
  parameter: apiKey
  sources:
  - openapi/moogsoft-alerts-incidents-openapi.yaml
  - openapi/moogsoft-azure-service-openapi.yaml
  - openapi/moogsoft-byo-api-service-openapi.yaml
  - openapi/moogsoft-cloudwatch-service-openapi.yaml
  - openapi/moogsoft-collectors-openapi.yaml
  - openapi/moogsoft-config-openapi.yaml
  - openapi/moogsoft-events-integration-openapi.yaml
  - openapi/moogsoft-incident-responder-openapi.yaml
  - openapi/moogsoft-metrics-integration-openapi.yaml
  - openapi/moogsoft-pagerduty-service-openapi.yaml
  - openapi/moogsoft-probable-rootcause-openapi.yaml
  - openapi/moogsoft-similar-incidents-openapi.yaml
  - openapi/moogsoft-ui-services-openapi.yaml
  - openapi/moogsoft-user-management-openapi.yaml
  - openapi/moogsoft-webhook-service-v2-openapi.yaml
  - openapi/moogsoft-workflow-engine-service-openapi.yaml
  type: apiKey
slug: moogsoft-authentication
source_filename: moogsoft-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-29'\nmethod: searched\nsource: https://api.docs.moogsoft.com/docs/latest/branches/main/8ae0406b4fb96-authentication, https://api.docs.moogsoft.com/docs/latest/branches/main/6553f9391961d-manage-api-keys,\n  https://api.docs.moogsoft.com/docs/latest/branches/main/b16f03ec715a2-user-roles-and-permissions, https://api.docs.moogsoft.com/docs/latest/branches/main/f86595eca2b25-request-requirements,\n  and openapi/ (17 contracts)\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: apiKey\n  description: API Key for accessing Alerts/Incidents API\n  sources:\n  - openapi/moogsoft-alerts-incidents-openapi.yaml\n  - openapi/moogsoft-azure-service-openapi.yaml\n  - openapi/moogsoft-byo-api-service-openapi.yaml\n  - openapi/moogsoft-cloudwatch-service-openapi.yaml\n  - openapi/moogsoft-collectors-openapi.yaml\n  - openapi/moogsoft-config-openapi.yaml\n  - openapi/moogsoft-events-integration-openapi.yaml\n\
  \  - openapi/moogsoft-incident-responder-openapi.yaml\n  - openapi/moogsoft-metrics-integration-openapi.yaml\n  - openapi/moogsoft-pagerduty-service-openapi.yaml\n  - openapi/moogsoft-probable-rootcause-openapi.yaml\n  - openapi/moogsoft-similar-incidents-openapi.yaml\n  - openapi/moogsoft-ui-services-openapi.yaml\n  - openapi/moogsoft-user-management-openapi.yaml\n  - openapi/moogsoft-webhook-service-v2-openapi.yaml\n  - openapi/moogsoft-workflow-engine-service-openapi.yaml\ndocs: https://api.docs.moogsoft.com/docs/latest/branches/main/8ae0406b4fb96-authentication\nmodel:\n  primary:\n    style: API key in a request header\n    header: apiKey\n    example: 'curl https://api.moogsoft.ai/v1/integrations/events -H ''Content-Type: application/json''\n      -H ''apiKey: <your-API-key>'''\n    declared_in: components.securitySchemes.ApiKeyAuth on all 17 contracts\n  alternative:\n    style: credentials embedded in the URL\n    form: https://<username>:<api_key>@api.moogsoft.ai/...\n    note:\
  \ Documented on the Authentication page as \"basic token authentication\". A bearer-token variant\n      is present in the docs source but commented out and therefore not offered.\n  oauth2:\n    supported_for_inbound_api: false\n    note: OAuth 2.0 appears in Moogsoft only for credentials Moogsoft uses to call OUT — webhook endpoint\n      auth (password grant, exclusive since 2024-11-18) and the external credential store (client credentials,\n      added 2025-04-29). There are no inbound OAuth scopes, so no scopes/ artifact is emitted.\n  console_sso:\n    issuer: https://auth.moogsoft.ai/\n    platform: Auth0\n    discovery: well-known/moogsoft-auth-openid-configuration.json\n    note: Governs sign-in to app.moogsoft.ai only. SAML/SSO configuration for the tenant is managed through\n      the SSO endpoints of the User Management API.\nkey_management:\n  creation: Settings > API Key Management in the console, or createApiKey (POST /v2/users/{userId}/keys).\n  ownership: A key always\
  \ belongs to the user who created it, even when another person uses it.\n  ceiling: A key can never be granted more permission than its creating user holds through roles and group\n    membership.\n  visibility: The secret is shown once at creation and is never retrievable afterwards.\n  revocation: Revoke in the console or delete via the API. Takes effect in about five minutes and cannot\n    be undone.\n  default: Users have no API key by default; one must be created explicitly.\n  orphans: Keys created by a deleted user remain active after that user is deleted.\n  docs: https://api.docs.moogsoft.com/docs/latest/branches/main/6553f9391961d-manage-api-keys\nauthorization:\n  model: role and permission based, enforced per feature area\n  default_roles:\n  - Operator (read-only, plus alert/incident status and ownership updates)\n  - Administrator (read and write)\n  - Owner (read and write)\n  custom_roles: true\n  group_roles: true\n  method_mapping:\n    GET: Read Only\n    POST: Full\
  \ Access\n    PATCH: Full Access\n    DELETE: Full Access\n  note: Permission failures can present as 404 rather than 403 on some resources.\n  docs: https://api.docs.moogsoft.com/docs/latest/branches/main/b16f03ec715a2-user-roles-and-permissions\ntransport:\n  https_only: true\n  tls: TLSv1.3 observed on www.moogsoft.com\n  mtls: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/moogsoft/refs/heads/main/authentication/moogsoft-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- AIOps
- Incident Management
- Observability
- Alerting
- Event Management
- Anomaly Detection
- Correlation
- On-Call
- Monitoring
- IT Operations
- DevOps
- SRE
---
