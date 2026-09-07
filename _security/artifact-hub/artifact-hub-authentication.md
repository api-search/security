---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: artifact-hub-organizations-api-openapi.yml
  format: yaml
  label: Artifact Hub Organizations API
  slug: artifact-hub-organizations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/artifact-hub/refs/heads/main/openapi/artifact-hub-organizations-api-openapi.yml
- filename: artifact-hub-packages-api-openapi.yml
  format: yaml
  label: Artifact Hub Packages API
  slug: artifact-hub-packages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/artifact-hub/refs/heads/main/openapi/artifact-hub-packages-api-openapi.yml
- filename: artifact-hub-repositories-api-openapi.yml
  format: yaml
  label: Artifact Hub Repositories API
  slug: artifact-hub-repositories-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/artifact-hub/refs/heads/main/openapi/artifact-hub-repositories-api-openapi.yml
- filename: artifact-hub-stats-api-openapi.yml
  format: yaml
  label: Artifact Hub Stats API
  slug: artifact-hub-stats-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/artifact-hub/refs/heads/main/openapi/artifact-hub-stats-api-openapi.yml
- filename: artifact-hub-subscriptions-api-openapi.yml
  format: yaml
  label: Artifact Hub Subscriptions API
  slug: artifact-hub-subscriptions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/artifact-hub/refs/heads/main/openapi/artifact-hub-subscriptions-api-openapi.yml
- filename: artifact-hub-users-api-openapi.yml
  format: yaml
  label: Artifact Hub Users API
  slug: artifact-hub-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/artifact-hub/refs/heads/main/openapi/artifact-hub-users-api-openapi.yml
- filename: artifact-hub-webhooks-api-openapi.yml
  format: yaml
  label: Artifact Hub Webhooks API
  slug: artifact-hub-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/artifact-hub/refs/heads/main/openapi/artifact-hub-webhooks-api-openapi.yml
- filename: artifact-hub-availability-checks-api-openapi.yml
  format: yaml
  label: Artifact Hub Availability checks API
  slug: artifact-hub-availability-checks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/artifact-hub/refs/heads/main/openapi/artifact-hub-availability-checks-api-openapi.yml
- filename: artifact-hub-integrations-api-openapi.yml
  format: yaml
  label: Artifact Hub Integrations API
  slug: artifact-hub-integrations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/artifact-hub/refs/heads/main/openapi/artifact-hub-integrations-api-openapi.yml
auth_types:
- apiKey
description: 'Artifact Hub uses a PAIRED API-KEY scheme: two headers, both required together, declared in the contract as a single security requirement {ApiKeyId: [], ApiKeySecret: []}. There is no OAuth 2.0 flow and no scopes on the API. Critically for an agent, there is no root-level `security` block — authentication is declared per operation, and the entire read surface (search, package and version detail for all 27 kinds, chart values, values schema, rendered templates, Trivy security reports, changelogs, stats and the bulk integration dumps) is ANONYMOUS. Credentials are needed only for account, organization, repository, subscription and webhook management.'
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Artifact Hub Authentication
name_suffix: Authentication
oauth_flows: []
overview: Artifact Hub secures its APIs with apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Artifact Hub
provider_slug: artifact-hub
scheme_count: 2
schemes:
- description: The API key identifier. Must be sent together with X-API-KEY-SECRET — sending one alone returns 401 exactly as sending neither does.
  in: header
  name: ApiKeyId
  parameter: X-API-KEY-ID
  required_with: ApiKeySecret
  sources:
  - openapi/_original/artifact-hub-openapi.yml
  type: apiKey
- description: The API key secret, paired with X-API-KEY-ID.
  in: header
  name: ApiKeySecret
  parameter: X-API-KEY-SECRET
  required_with: ApiKeyId
  sources:
  - openapi/_original/artifact-hub-openapi.yml
  type: apiKey
slug: artifact-hub-authentication
source_filename: artifact-hub-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-04'\nmethod: searched\nsource: >-\n  openapi/_original/artifact-hub-openapi.yml (v1.23.0) components.securitySchemes and the\n  per-operation security blocks, plus https://artifacthub.io/docs/topics/authorization/ and\n  https://artifacthub.io/docs/topics/faq/ (fetched 2026-09-04)\ndocs: https://artifacthub.io/docs/topics/authorization/\nreference: https://artifacthub.io/docs/api/\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\n  paired: true\n  anonymous_read_surface: true\ndescription: >-\n  Artifact Hub uses a PAIRED API-KEY scheme: two headers, both required together, declared in\n  the contract as a single security requirement {ApiKeyId: [], ApiKeySecret: []}. There is no\n  OAuth 2.0 flow and no scopes on the API. Critically for an agent, there is no root-level\n  `security` block — authentication is declared per operation, and the entire read surface\n  (search, package and version detail for all 27 kinds, chart values, values schema,\
  \ rendered\n  templates, Trivy security reports, changelogs, stats and the bulk integration dumps) is\n  ANONYMOUS. Credentials are needed only for account, organization, repository, subscription\n  and webhook management.\nschemes:\n- name: ApiKeyId\n  type: apiKey\n  in: header\n  parameter: X-API-KEY-ID\n  required_with: ApiKeySecret\n  description: >-\n    The API key identifier. Must be sent together with X-API-KEY-SECRET — sending one alone\n    returns 401 exactly as sending neither does.\n  sources:\n  - openapi/_original/artifact-hub-openapi.yml\n- name: ApiKeySecret\n  type: apiKey\n  in: header\n  parameter: X-API-KEY-SECRET\n  required_with: ApiKeyId\n  description: The API key secret, paired with X-API-KEY-ID.\n  sources:\n  - openapi/_original/artifact-hub-openapi.yml\ncredential_lifecycle:\n  issuance: >-\n    API keys are created in the Artifact Hub web control panel after signing in. The public\n    v1.23.0 contract exposes NO key-management operations — there is no /api-keys\
  \ path — so an\n    agent cannot mint, rotate or revoke a key programmatically. This is a real onboarding\n    ceiling: a human must visit the site once.\n  rotation: not documented\n  expiry: not documented\n  revocation: control panel only\nhuman_sign_in:\n  note: >-\n    Distinct from API authentication. Users sign in to the web application with email and\n    password, with optional TOTP two-factor (User.tfa_enabled, recovery codes issued at\n    setup). A self-hosted deployment can additionally sign users in through an OpenID Connect\n    provider (hub.server.oauth.oidc). Custom OAuth providers are explicitly not supported.\n    None of this applies to API calls.\nauthorization:\n  model: Open Policy Agent (rego) policies evaluated per organization\n  docs: https://artifacthub.io/docs/topics/authorization/\n  default: >-\n    Disabled. With authorization off, every member of an organization may perform every\n    action on it.\n  predefined_policies:\n  - id: rbac.v1\n    description:\
  \ >-\n      The only predefined policy. A roles-based policy where the organization supplies a JSON\n      data file mapping roles to users and to allowed actions; the `owner` role implies the\n      action `all`.\n  custom_policies: >-\n    An organization may instead supply its own rego policy plus a JSON data file, both managed\n    through getOrganizationAuthPolicy / updateOrganizationAuthPolicy.\n  actions:\n  - all\n  - addOrganizationMember\n  - addOrganizationRepository\n  - deleteOrganization\n  - deleteOrganizationMember\n  - deleteOrganizationRepository\n  - getAuthorizationPolicy\n  - transferOrganizationRepository\n  - updateAuthorizationPolicy\n  - updateOrganization\n  - updateOrganizationRepository\n  introspection:\n    operation: getAllowedActions\n    path: GET /orgs/{orgName}/user-allowed-actions\n    note: >-\n      The permission-discovery endpoint an agent should call before attempting an\n      organization write, rather than discovering the denial as a 403.\n \
  \ scopes: none\n  scopes_note: >-\n    These action names are policy inputs, not token scopes. No OAuth scopes artifact is\n    written for this provider because the API declares no oauth2 security scheme and the docs\n    document no OAuth flow for API access.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/artifact-hub/refs/heads/main/authentication/artifact-hub-authentication.yml
summary_line: apiKey · 2 schemes
tags:
- Cloud-Native
- CNCF
- Helm Charts
- Package Registry
- Discovery
- Open-Source
---
