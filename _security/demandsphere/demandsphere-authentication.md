---
api_key_in:
- query
api_specs:
- filename: demandsphere-keywords-api-openapi.yml
  format: yaml
  label: DemandSphere Keywords API
  slug: demandsphere-keywords-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/demandsphere/refs/heads/main/openapi/demandsphere-keywords-api-openapi.yml
- filename: demandsphere-pages-api-openapi.yml
  format: yaml
  label: DemandSphere Pages API
  slug: demandsphere-pages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/demandsphere/refs/heads/main/openapi/demandsphere-pages-api-openapi.yml
- filename: demandsphere-searchengines-api-openapi.yml
  format: yaml
  label: DemandSphere SearchEngines API
  slug: demandsphere-searchengines-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/demandsphere/refs/heads/main/openapi/demandsphere-searchengines-api-openapi.yml
- filename: demandsphere-sites-api-openapi.yml
  format: yaml
  label: DemandSphere Sites API
  slug: demandsphere-sites-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/demandsphere/refs/heads/main/openapi/demandsphere-sites-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Demandsphere Authentication
name_suffix: Authentication
oauth_flows: []
overview: DemandSphere secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: DemandSphere
provider_slug: demandsphere
scheme_count: 1
schemes:
- in: query
  name: ApiKey
  parameter: api_key
  sources:
  - openapi/demandsphere-keywords-api-openapi.yml
  - openapi/demandsphere-pages-api-openapi.yml
  - openapi/demandsphere-searchengines-api-openapi.yml
  - openapi/demandsphere-sites-api-openapi.yml
  type: apiKey
slug: demandsphere-authentication
source_filename: demandsphere-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: searched\nsource: openapi/demandsphere-keywords-api-openapi.yml, openapi/demandsphere-pages-api-openapi.yml,\n  openapi/demandsphere-searchengines-api-openapi.yml, openapi/demandsphere-sites-api-openapi.yml\ndocs: https://www.demandsphere.com/platform/apis/rest-apis/\nkey_issuance: app.demandsphere.com/settings\nkey_issuance_source: https://github.com/DemandSphereDev/demandsphere-mcp (tools/utils.py auth_error recovery hint)\ndocs_discrepancy: >-\n  https://www.demandsphere.com/platform/apis/rest-apis/ advertises \"OAuth 2.0\n  Authentication\" for the REST API. No OAuth flow, authorization endpoint or\n  scope registry is published for api.demandsphere.com, the OpenAPI declares only\n  an apiKey-in-query scheme, and DemandSphere's own first-party MCP client sends\n  the credential as the `api_key` query parameter. The company does run OAuth/OIDC\n  — a Keycloak realm at auth.demandsphere.com serving the web application and\n  help-center SSO\
  \ — but it does not front the API.\nsso:\n  provider: Keycloak\n  realm: https://auth.demandsphere.com/auth/realms/DemandSphere\n  discovery: well-known/demandsphere-openid-configuration.json\n  scope: application and help-center sign-in only; not an API authorization server.\ntransport_note: >-\n  The credential travels in the URL query string, so it can be captured in\n  reverse-proxy, CDN and monitoring logs — DemandSphere documents this risk in\n  its MCP server README and recommends stripping query strings from access logs.\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - query\nschemes:\n- name: ApiKey\n  type: apiKey\n  in: query\n  parameter: api_key\n  sources:\n  - openapi/demandsphere-keywords-api-openapi.yml\n  - openapi/demandsphere-pages-api-openapi.yml\n  - openapi/demandsphere-searchengines-api-openapi.yml\n  - openapi/demandsphere-sites-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/demandsphere/refs/heads/main/authentication/demandsphere-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- SEO
- Search Intelligence
- SERP Analytics
- AI Search
- LLM Visibility
- Rank Tracking
- Analytics
- API
- MCP
---
