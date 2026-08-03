---
api_key_in:
- header
api_specs:
- filename: bigeye-metadata-openapi.json
  format: json
  label: Bigeye Metadata API
  slug: bigeye-metadata-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bigeye/refs/heads/main/openapi/bigeye-metadata-openapi.json
- filename: bigeye-observability-openapi.json
  format: json
  label: Bigeye Observability API
  slug: bigeye-observability-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bigeye/refs/heads/main/openapi/bigeye-observability-openapi.json
- filename: bigeye-sensitivity-openapi.json
  format: json
  label: Bigeye Sensitivity API
  slug: bigeye-sensitivity-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bigeye/refs/heads/main/openapi/bigeye-sensitivity-openapi.json
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: searched
name: Bigeye Authentication
name_suffix: Authentication
oauth_flows: []
overview: Bigeye secures its APIs with apiKey and http across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Bigeye
provider_slug: bigeye
scheme_count: 3
schemes:
- description: HTTP Basic with a Bigeye username and password.
  name: basicAuth
  scheme: basic
  sources:
  - openapi/bigeye-metadata-openapi.json
  - openapi/bigeye-observability-openapi.json
  - openapi/bigeye-sensitivity-openapi.json
  type: http
- description: Add 'apikey ' to the beginning of your api key
  in: header
  name: Personal_API_Key
  parameter: Authorization
  sources:
  - openapi/bigeye-metadata-openapi.json
  - openapi/bigeye-observability-openapi.json
  - openapi/bigeye-sensitivity-openapi.json
  type: apiKey
- description: Add 'apikey ' to the beginning of your api key
  in: header
  name: Agent_API_Key
  parameter: Authorization
  sources:
  - openapi/bigeye-metadata-openapi.json
  - openapi/bigeye-observability-openapi.json
  - openapi/bigeye-sensitivity-openapi.json
  type: apiKey
slug: bigeye-authentication
source_filename: bigeye-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-02'\nmethod: searched\nsource: openapi/bigeye-metadata-openapi.json, openapi/bigeye-observability-openapi.json,\n  openapi/bigeye-sensitivity-openapi.json\ndocs: https://docs.bigeye.com/docs/using-api-keys\nadditional_docs:\n- https://docs.bigeye.com/docs/api-user-guide\n- https://docs.bigeye.com/docs/service-accounts\n- https://docs.bigeye.com/docs/permissions\n- https://docs.bigeye.com/docs/single-sign-on-sso\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\n  oauth2_flows: []\n  oauth2: false\n  note: >-\n    Bigeye has no OAuth surface for its API. The three published OpenAPI\n    definitions declare exactly three security schemes, applied identically\n    across all 263 operations, with a top-level requirement of\n    [basicAuth] OR [Personal_API_Key].\nschemes:\n- name: basicAuth\n  type: http\n  scheme: basic\n  description: HTTP Basic with a Bigeye username and password.\n  sources:\n  - openapi/bigeye-metadata-openapi.json\n\
  \  - openapi/bigeye-observability-openapi.json\n  - openapi/bigeye-sensitivity-openapi.json\n- name: Personal_API_Key\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: Add 'apikey ' to the beginning of your api key\n  sources:\n  - openapi/bigeye-metadata-openapi.json\n  - openapi/bigeye-observability-openapi.json\n  - openapi/bigeye-sensitivity-openapi.json\n- name: Agent_API_Key\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: Add 'apikey ' to the beginning of your api key\n  sources:\n  - openapi/bigeye-metadata-openapi.json\n  - openapi/bigeye-observability-openapi.json\n  - openapi/bigeye-sensitivity-openapi.json\ncredential_types:\n- name: Personal API Key\n  bound_to: an individual user account\n  managed_at: https://app.bigeye.com/settings/api-keys\n  create: Advanced Settings > API Keys > \"Create personal key\"\n  verify_endpoint: GET https://<company-prefix>.bigeye.com/api/v1/personal-api-keys/verify\n  verify_success: 204\n \
  \ verify_failure: 401\n  example_prefix: bigeye_pak_\n  shown_once: true\n  operations: [ApiKeyService_GetAllPersonalApiKeys, ApiKeyService_DeletePersonalApiKey,\n    ApiKeyService_VerifyPersonalApiKey]\n- name: Agent API Key\n  bound_to: the company, used by the Bigeye data source agent\n  managed_at: https://app.bigeye.com/settings/api-keys\n  create: Advanced Settings > API Keys > \"Create Agent key\"\n  admin_only: true\n  verify_endpoint: GET https://app.bigeye.com/api/v1/agent-api-keys/verify\n  verify_success: 204\n  verify_failure: 401\n  shown_once: true\n  operations: [ApiKeyService_GetAllAgentApiKeys, ApiKeyService_CreateAgentApiKey, ApiKeyService_DeleteAgentApiKey,\n    ApiKeyService_VerifyAgentApiKey]\n  note: Replaces the older mTLS agent authentication — see https://docs.bigeye.com/docs/upgrading-agent-from-mtls-to-api-keys\n- name: Service Account API Key\n  bound_to: a non-human identity used to automate workflows\n  docs: https://docs.bigeye.com/docs/service-accounts\n\
  \  operations: [ServiceAccountApiKeyService_CreateServiceAccountApiKey, ServiceAccountApiKeyService_DeleteServiceAccountApiKey,\n    ServiceAccountApiKeyService_ListAllServiceAccountKeys, ServiceAccountApiKeyService_ListKeysForServiceAccount]\nheader_format:\n  header: Authorization\n  value: apikey <API_KEY>\n  warning: >-\n    The prefix is the literal lowercase string \"apikey \" — NOT \"Bearer\" and NOT\n    \"ApiKey\". This is the most common integration mistake against the Bigeye\n    API and is the same header the MCP gateway expects.\n  example: 'curl -i -H \"Authorization: apikey $BIGEYE_PERSONAL_API_KEY\" \"https://app.bigeye.com/api/v1/personal-api-keys/verify\"'\nauthorization:\n  model: role-based, evaluated per workspace\n  roles: [view only, edit, manage, admin]\n  docs: https://docs.bigeye.com/docs/permissions\n  note: >-\n    \"The access level for authentication is based upon the access granted in\n    Bigeye. Users with the view only, edit, and manage roles will be restricted\n\
  \    from doing certain API calls based upon their access.\" The API therefore\n    returns different results for the same operation depending on the caller's\n    role, and the OpenAPI cannot express which operations a role can reach.\n  scopes: false\n  scopes_note: >-\n    There are no OAuth scopes. Authorization is entirely role-based, which is\n    why no scopes/ artifact is emitted for this provider.\ntenancy_header:\n  header: X-Bigeye-Workspace-Id\n  required_for: workspace-scoped list, count and create operations\n  alternatives: [workspaceId query parameter, workspaceId body parameter]\n  failure: 400 '{\"code\":400,\"message\":\"A workspace ID must be supplied\"}'\nother_surfaces:\n- surface: MCP Gateway\n  url: https://mcpgateway.bigeye.com/mcp\n  auth: 'Authorization: apikey <key> + x-bigeye-workspace-id: <id> (+ optional x-bigeye-url)'\n  oauth: false\n  artifact: mcp/bigeye-mcp.yml\n- surface: Bigeye CLI\n  auth: basic (username/password) or browser session reuse, via `bigeye\
  \ configure`\n  credential_file: ~/.bigeye/credentials\n  artifact: cli/bigeye-cli.yml\n- surface: Application sign-in (not the API)\n  auth: 'SSO via Auth0: Okta, Ping Identity and Azure AD supported for Enterprise'\n  docs: https://docs.bigeye.com/docs/single-sign-on-sso\n- surface: Data source connections (Bigeye to the customer's warehouse)\n  auth: read-only JDBC service accounts, Kerberos supported on agent connections,\n    OAuth client-credentials for Salesforce sources\n  docs: https://docs.bigeye.com/docs/source-support\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bigeye/refs/heads/main/authentication/bigeye-authentication.yml
summary_line: apiKey/http · 3 schemes
tags:
- Company
- Data Observability
- Data Quality
- Data Lineage
- Data Governance
- Metadata Management
- Data Catalog
- Sensitive Data Discovery
- Monitoring
- Analytics
- AI Trust
- Snowflake
- Databricks
---
