---
api_key_in: []
api_specs:
- filename: abbyy-vantage-processing-openapi.yml
  format: yaml
  label: ABBYY Vantage Processing REST API
  slug: abbyy-vantage-processing
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/abbyy/refs/heads/main/openapi/abbyy-vantage-processing-openapi.yml
- filename: abbyy-vantage-reporting-openapi.yml
  format: yaml
  label: ABBYY Vantage Reporting API
  slug: abbyy-vantage-reporting
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/abbyy/refs/heads/main/openapi/abbyy-vantage-reporting-openapi.yml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Abbyy Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: ABBYY secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: ABBYY
provider_slug: abbyy
scheme_count: 1
schemes:
- flows:
  - authorizationUrl: https://vantage-us.abbyy.com/auth2/connect/authorize
    flow: authorizationCode
    scopes: 3
    tokenUrl: https://vantage-us.abbyy.com/auth2/connect/token
  name: OAuth2Security
  sources:
  - openapi/abbyy-vantage-processing-openapi.yml
  - openapi/abbyy-vantage-reporting-openapi.yml
  - openapi/abbyy-vantage-reporting-v1-openapi.yml
  type: oauth2
slug: abbyy-authentication
source_filename: abbyy-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-29'\nmethod: searched\nsource: https://docs.abbyy.com/vantage/developer/authentication/authentication + openapi/_original/abbyy-vantage-processing-openapi.json\n  (fetched https://docs.abbyy.com/openapi.json, HTTP 200)\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: OAuth2Security\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://vantage-us.abbyy.com/auth2/connect/authorize\n    tokenUrl: https://vantage-us.abbyy.com/auth2/connect/token\n    scopes: 3\n  sources:\n  - openapi/abbyy-vantage-processing-openapi.yml\n  - openapi/abbyy-vantage-reporting-openapi.yml\n  - openapi/abbyy-vantage-reporting-v1-openapi.yml\ndocs: https://docs.abbyy.com/vantage/developer/authentication/authentication\nnote: The Vantage OpenAPI declares only the OAuth 2.0 authorization-code flow, but ABBYY documents three flows for\n  the same token endpoint. Bearer token goes in the Authorization header on\
  \ every request. The FlexiCapture Cloud\n  for Invoices API is a separate surface using HTTP Basic auth with an application id and token, base64-encoded.\ndocumented_flows:\n- flow: authorizationCode\n  pkce: true\n  best_for: User-facing applications\n  docs: https://docs.abbyy.com/vantage/developer/authentication/authorization-code-flow\n- flow: clientCredentials\n  best_for: Machine-to-machine integrations\n  docs: https://docs.abbyy.com/vantage/developer/authentication/client-credentials\n- flow: password\n  best_for: Server-to-server integrations (Resource Owner Password Credentials)\n  docs: https://docs.abbyy.com/vantage/developer/authentication/resource-owner-password-credentials\ntoken_endpoints:\n- region: US\n  authorizationUrl: https://vantage-us.abbyy.com/auth2/connect/authorize\n  tokenUrl: https://vantage-us.abbyy.com/auth2/connect/token\n- region: EU\n  authorizationUrl: https://vantage-eu.abbyy.com/auth2/connect/authorize\n  tokenUrl: https://vantage-eu.abbyy.com/auth2/connect/token\n\
  - region: AU\n  authorizationUrl: https://vantage-au.abbyy.com/auth2/connect/authorize\n  tokenUrl: https://vantage-au.abbyy.com/auth2/connect/token\nother_surfaces:\n- api: ABBYY FlexiCapture Cloud for Invoices API\n  type: http\n  scheme: basic\n  credential: application id + token, colon-joined and base64-encoded\n  docs: https://docs.abbyy.com/flexi-capture/cloud/cloud-f-cfor-invoices-api-auth\n- api: ABBYY Documentation MCP Server\n  type: none\n  credential: anonymous — no token required\n  docs: https://docs.abbyy.com/vantage/developer/mcp-server\nonboarding:\n  self_serve: false\n  note: A Vantage tenant is provisioned by ABBYY on request; API clients are then created by the tenant admin under\n    Administration > API clients.\n  request_url: https://www.abbyy.com/company/contact-us/\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/abbyy/refs/heads/main/authentication/abbyy-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- AI Automation
- Document Processing
- OCR
- Intelligent Document Processing
- Data Extraction
- Process Intelligence
- MCP
- Agent Skills
- RPA
- Enterprise Automation
---
