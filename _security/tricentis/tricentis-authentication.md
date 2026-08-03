---
api_key_in:
- header
- query
api_specs:
- filename: tricentis-qtest-manager-openapi.yaml
  format: yaml
  label: qTest Manager API v3
  slug: qtest-manager
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tricentis/refs/heads/main/openapi/tricentis-qtest-manager-openapi.yaml
- filename: tricentis-qtest-parameters-openapi.yaml
  format: yaml
  label: qTest Parameters API
  slug: qtest-parameters
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tricentis/refs/heads/main/openapi/tricentis-qtest-parameters-openapi.yaml
- filename: tricentis-qtest-pulse-openapi.yaml
  format: yaml
  label: qTest Pulse API
  slug: qtest-pulse
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tricentis/refs/heads/main/openapi/tricentis-qtest-pulse-openapi.yaml
- filename: tricentis-qtest-scenario-openapi.yaml
  format: yaml
  label: qTest Scenario API
  slug: qtest-scenario
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tricentis/refs/heads/main/openapi/tricentis-qtest-scenario-openapi.yaml
- filename: tricentis-qtest-sessions-openapi.yaml
  format: yaml
  label: qTest Explorer Sessions API
  slug: qtest-sessions
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tricentis/refs/heads/main/openapi/tricentis-qtest-sessions-openapi.yaml
- filename: tricentis-qtest-data-export-openapi.yaml
  format: yaml
  label: qTest Data Export API
  slug: qtest-data-export
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tricentis/refs/heads/main/openapi/tricentis-qtest-data-export-openapi.yaml
- filename: tricentis-qtest-analytics-openapi.json
  format: json
  label: Tricentis Analytics API
  slug: analytics
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tricentis/refs/heads/main/openapi/tricentis-qtest-analytics-openapi.json
- filename: tricentis-neoload-openapi.yaml
  format: yaml
  label: NeoLoad API v3
  slug: neoload
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tricentis/refs/heads/main/openapi/tricentis-neoload-openapi.yaml
- filename: tricentis-ttm4j-openapi.json
  format: json
  label: Tricentis Test Management for Jira API
  slug: ttm4j
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tricentis/refs/heads/main/openapi/tricentis-ttm4j-openapi.json
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: searched
name: Tricentis Authentication
name_suffix: Authentication
oauth_flows: []
overview: Tricentis secures its APIs with apiKey and http across 6 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Tricentis
provider_slug: tricentis
scheme_count: 6
schemes:
- in: header
  name: NeoloadAuthorizer
  parameter: accountToken
  sources:
  - openapi/tricentis-neoload-openapi.yaml
  type: apiKey
- name: BasicAuth
  scheme: basic
  sources:
  - openapi/tricentis-qtest-analytics-openapi.json
  type: http
- in: query
  name: ApiKeyAuth
  parameter: apikey
  sources:
  - openapi/tricentis-qtest-analytics-openapi.json
  type: apiKey
- in: header
  name: Authorization
  parameter: Authorization
  sources:
  - openapi/tricentis-qtest-manager-openapi.yaml
  - openapi/tricentis-qtest-pulse-openapi.yaml
  - openapi/tricentis-qtest-sessions-openapi.yaml
  - openapi/tricentis-ttm4j-openapi.json
  type: apiKey
- in: header
  name: token
  parameter: x-access-token
  sources:
  - openapi/tricentis-qtest-parameters-openapi.yaml
  type: apiKey
- in: header
  name: qtestUrl
  parameter: x-qtest-url
  sources:
  - openapi/tricentis-qtest-pulse-openapi.yaml
  type: apiKey
slug: tricentis-authentication
source_filename: tricentis-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-02'\nmethod: searched\nsource: openapi/tricentis-neoload-openapi.yaml, openapi/tricentis-qtest-analytics-openapi.json,\n  openapi/tricentis-qtest-manager-openapi.yaml, openapi/tricentis-qtest-parameters-openapi.yaml,\n  openapi/tricentis-qtest-pulse-openapi.yaml, openapi/tricentis-qtest-sessions-openapi.yaml, openapi/tricentis-ttm4j-openapi.json\n  + provider auth documentation\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\n  - query\n  oauth2_flows: []\n  note: Tricentis authenticates every REST product with a header-carried credential and declares\n    none of them as oauth2 in the specs, even where an OAuth token endpoint exists. qTest issues\n    a bearer token from POST /oauth/token but models it as an apiKey header named Authorization.\n    The only true OAuth surface is the Tosca Cloud identity service used by the Tosca Cloud MCP\n    server and toscactl - see scopes/tricentis-scopes.yml.\nschemes:\n- name: NeoloadAuthorizer\n\
  \  type: apiKey\n  in: header\n  parameter: accountToken\n  sources:\n  - openapi/tricentis-neoload-openapi.yaml\n- name: BasicAuth\n  type: http\n  scheme: basic\n  sources:\n  - openapi/tricentis-qtest-analytics-openapi.json\n- name: ApiKeyAuth\n  type: apiKey\n  in: query\n  parameter: apikey\n  sources:\n  - openapi/tricentis-qtest-analytics-openapi.json\n- name: Authorization\n  type: apiKey\n  in: header\n  parameter: Authorization\n  sources:\n  - openapi/tricentis-qtest-manager-openapi.yaml\n  - openapi/tricentis-qtest-pulse-openapi.yaml\n  - openapi/tricentis-qtest-sessions-openapi.yaml\n  - openapi/tricentis-ttm4j-openapi.json\n- name: token\n  type: apiKey\n  in: header\n  parameter: x-access-token\n  sources:\n  - openapi/tricentis-qtest-parameters-openapi.yaml\n- name: qtestUrl\n  type: apiKey\n  in: header\n  parameter: x-qtest-url\n  sources:\n  - openapi/tricentis-qtest-pulse-openapi.yaml\ndocs:\n- https://docs.tricentis.com/qtest-saas/content/apis/overview/qtest_api_specification.htm\n\
  - https://docs.tricentis.com/ttm-for-jira/content/developer/api_authorization.htm\n- https://docs.tricentis.com/tosca-cloud/en-us/content/ai_integration/connect_mcp_server.htm\ntoken_endpoints:\n- api: qTest Manager\n  operation: postAccessToken\n  path: POST /oauth/token\n  summary: Log in\n  source: openapi/tricentis-qtest-manager-openapi.yaml\n- api: qTest Manager\n  operation: tokenStatus\n  path: GET /oauth/status\n  summary: Gets status of access token\n  source: openapi/tricentis-qtest-manager-openapi.yaml\ncredential_sources:\n- api: qTest\n  where: qTest Resources page, API & SDK section\n  docs: https://docs.tricentis.com/qtest-saas/content/apis/overview/how_to_use_interactive_api_documentation.htm\n- api: Tricentis Test Management for Jira\n  where: TTM4J API authorization settings in Jira\n  docs: https://docs.tricentis.com/ttm-for-jira/content/developer/api_authorization.htm\n  validate: HEAD /v1/api-key/is-alive\n- api: NeoLoad\n  where: NeoLoad Web account settings (accountToken)\n\
  non_spec_surfaces:\n- surface: Tosca Cloud identity\n  type: oauth2\n  flows:\n  - authorizationCode+PKCE\n  - deviceCode\n  - clientCredentials\n  client_id: MCPServer\n  scope: tta\n  docs: https://docs.tricentis.com/tosca-cloud/en-us/content/ai_integration/connect_mcp_server.htm\n- surface: Tosca Commander in-process MCP\n  type: none\n  note: localhost-bound on default port 46248\nmfa_sso:\n  note: Tricentis cloud products support enterprise SSO/SAML at the tenant level; no SSO metadata\n    is published anonymously.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tricentis/refs/heads/main/authentication/tricentis-authentication.yml
summary_line: apiKey/http · 6 schemes
tags:
- Company
- Testing
- Test Automation
- Quality Engineering
- Test Management
- Performance Testing
- Continuous Testing
- DevOps
- SAP
- Data Integrity
- Agentic Testing
---
