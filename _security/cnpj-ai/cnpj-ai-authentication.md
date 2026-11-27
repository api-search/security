---
anonymous_access: false
api_key_in: []
api_specs:
- filename: cnpj-ai-cat-logo-api-openapi.yml
  format: yaml
  label: cnpj.ai Catálogo API
  slug: cnpj-ai-cat-logo-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cnpj-ai/openapi/cnpj-ai-cat-logo-api-openapi.yml
- filename: cnpj-ai-consulta-de-cnpj-api-openapi.yml
  format: yaml
  label: cnpj.ai Consulta de CNPJ API
  slug: cnpj-ai-consulta-de-cnpj-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cnpj-ai/openapi/cnpj-ai-consulta-de-cnpj-api-openapi.yml
- filename: cnpj-ai-empresas-api-openapi.yml
  format: yaml
  label: cnpj.ai Empresas API
  slug: cnpj-ai-empresas-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cnpj-ai/openapi/cnpj-ai-empresas-api-openapi.yml
- filename: cnpj-ai-empresas-fontes-api-openapi.yml
  format: yaml
  label: cnpj.ai empresas — fontes API
  slug: cnpj-ai-empresas-fontes-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cnpj-ai/openapi/cnpj-ai-empresas-fontes-api-openapi.yml
- filename: cnpj-ai-estabelecimentos-api-openapi.yml
  format: yaml
  label: cnpj.ai Estabelecimentos API
  slug: cnpj-ai-estabelecimentos-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cnpj-ai/openapi/cnpj-ai-estabelecimentos-api-openapi.yml
- filename: cnpj-ai-estabelecimentos-fontes-api-openapi.yml
  format: yaml
  label: cnpj.ai estabelecimentos — fontes API
  slug: cnpj-ai-estabelecimentos-fontes-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cnpj-ai/openapi/cnpj-ai-estabelecimentos-fontes-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: cnpj.ai Authentication
name_suffix: Authentication
oauth_flows: []
overview: cnpj.ai secures its APIs with http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: cnpj.ai
provider_slug: cnpj-ai
scheme_count: 2
schemes:
- header: 'Authorization: Bearer <API_KEY>'
  name: ChaveAPI
  notes: Key created in the cnpj.ai account (https://cnpj.ai/conta); shown only once; up to 5 active keys; revocable. Same key for v1, v2 and the MCP server. Backend-only; CORS not enabled.
  scheme: bearer
  sources:
  - openapi/cnpj-ai-v1-openapi.yml
  - openapi/cnpj-ai-v2-openapi.yml
  type: http
- applies_to: https://mcp.cnpj.ai/mcp
  name: MCP OAuth
  notes: The MCP server documents "OAuth 2.1 ou API key"; clients open the cnpj.ai OAuth login automatically, or send Authorization Bearer with an API key. Not used by the REST API contracts.
  source: https://mcp.cnpj.ai/
  type: oauth2
slug: cnpj-ai-authentication
source_filename: cnpj-ai-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: searched\nsource: https://cnpj.ai/api/docs\ndocs: https://cnpj.ai/api/docs\nsummary:\n  types:\n  - http\nschemes:\n- name: ChaveAPI\n  type: http\n  scheme: bearer\n  header: 'Authorization: Bearer <API_KEY>'\n  sources:\n  - openapi/cnpj-ai-v1-openapi.yml\n  - openapi/cnpj-ai-v2-openapi.yml\n  notes: Key created in the cnpj.ai account (https://cnpj.ai/conta); shown only once; up to 5 active keys; revocable. Same key for v1, v2 and the MCP server. Backend-only; CORS not enabled.\n- name: MCP OAuth\n  type: oauth2\n  applies_to: https://mcp.cnpj.ai/mcp\n  source: https://mcp.cnpj.ai/\n  notes: The MCP server documents \"OAuth 2.1 ou API key\"; clients open the cnpj.ai OAuth login automatically, or send Authorization Bearer with an API key. Not used by the REST API contracts.\n"
source_yaml_url: https://artifacts.apis.io/cnpj-ai/authentication/cnpj-ai-authentication.yml
summary_line: http · 2 schemes
tags:
- Company
- Company Data
- Brazil
- CNPJ
- Open Data
- Public Records
- Business Registry
- Compliance
- MCP
---
