---
anonymous_access: true
api_key_in: []
api_specs:
- filename: caspar-manufaktur-de-caspar-manufaktur-api-materialien-nlweb-und-projekt-bergaben-api-openapi.yml
  format: yaml
  label: Caspar Manufaktur Caspar Manufaktur API – Materialien, NLWeb Und Projektübergaben API
  slug: caspar-manufaktur-de-caspar-manufaktur-api-materialien-nlweb-und-projekt-bergaben-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/caspar-manufaktur-de/openapi/caspar-manufaktur-de-caspar-manufaktur-api-materialien-nlweb-und-projekt-bergaben-api-openapi.yml
- filename: caspar-manufaktur-de-health-api-openapi.yml
  format: yaml
  label: Caspar Manufaktur Health API
  slug: caspar-manufaktur-de-health-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/caspar-manufaktur-de/openapi/caspar-manufaktur-de-health-api-openapi.yml
- filename: caspar-manufaktur-de-mcp-api-openapi.yml
  format: yaml
  label: Caspar Manufaktur MCP API
  slug: caspar-manufaktur-de-mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/caspar-manufaktur-de/openapi/caspar-manufaktur-de-mcp-api-openapi.yml
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 0
method: searched
name: Caspar Manufaktur Authentication
name_suffix: Authentication
oauth_flows: []
overview: Caspar Manufaktur declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Caspar Manufaktur
provider_slug: caspar-manufaktur-de
scheme_count: 1
schemes:
- applies_to:
  - askQuestion
  - askQuestionPost
  - askQuestionStream
  - getMcpInfo
  - listMaterials
  - recommendMaterial
  - getCompanyInformation
  - getApiIndex
  - getApiHealth
  - createProjectHandoff
  description: 'Read endpoints need no API key: materials, material recommendation, company data and NLWeb /ask'
  type: none
slug: caspar-manufaktur-de-authentication
source_filename: caspar-manufaktur-de-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-03'\nmethod: searched\nsource: https://www.caspar-manufaktur.de/auth.md\ndocs: https://www.caspar-manufaktur.de/auth.md\nsummary: Public read endpoints, NLWeb /ask and the MCP server need no authentication. No API keys, OAuth flow or self-service registration exist; the OpenAPI declares no securitySchemes.\nschemes:\n- type: none\n  description: \"Read endpoints need no API key: materials, material recommendation, company data and NLWeb /ask\"\n  applies_to: [askQuestion, askQuestionPost, askQuestionStream, getMcpInfo, listMaterials, recommendMaterial, getCompanyInformation, getApiIndex, getApiHealth, createProjectHandoff]\nagent_auth: not_supported\nnotes:\n- \"No token, API key, or OAuth credential is issued. Access is project-scoped and human-approved.\"\n- FTP credentials for print-file upload are issued by a person after order confirmation (outside the API).\n- MCP server (Streamable HTTP, no auth) at https://www.caspar-manufaktur.de/mcp/\n"
source_yaml_url: https://artifacts.apis.io/caspar-manufaktur-de/authentication/caspar-manufaktur-de-authentication.yml
summary_line: 1 scheme
tags:
- Company
- Manufacturing
- Wallpaper
- Digital Printing
- Interior Design
- B2B
- White Label
- Germany
- MCP
- AI Agents
---
