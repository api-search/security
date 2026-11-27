---
anonymous_access: false
api_key_in: []
api_specs:
- filename: emisso-ai-openapi.json
  format: json
  label: Emisso API
  slug: emisso-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/emisso-ai/openapi/emisso-ai-openapi.json
auth_types: []
description: Authentication uses an API key provided as a Bearer token in the Authorization header.
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Emisso Authentication
name_suffix: Authentication
oauth_flows: []
overview: Emisso declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Emisso
provider_slug: emisso-ai
scheme_count: 1
schemes:
- evidence: 'curl -X POST https://connect.emisso.ai/api/v1/tools/conexiones.estado.consultar/execute \ -H "Authorization: Bearer $EMISSO_CONNECT_API_KEY " \ -H "Content-Type: application/json" \ -d ''{"input": {}}'''
  header: Authorization
  how_to_obtain: Create an API key in connect.emisso.ai/api-keys and copy the secret that starts with connect_sk_…
  location: header
  name: Authorization
  type: http-bearer
slug: emisso-ai-authentication
source_filename: emisso-ai-authentication.yml
source_heading: Authentication Profile
source_url: https://connect.emisso.ai/docs/empezar/primera-llamada
source_yaml: "generated: '2026-11-06'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://connect.emisso.ai/docs/empezar/primera-llamada\nsources:\n- https://connect.emisso.ai/docs/empezar/primera-llamada\ndescription: Authentication uses an API key provided as a Bearer token in the Authorization header.\nschemes:\n- type: http-bearer\n  name: Authorization\n  evidence: 'curl -X POST https://connect.emisso.ai/api/v1/tools/conexiones.estado.consultar/execute \\ -H \"Authorization: Bearer $EMISSO_CONNECT_API_KEY\n    \" \\ -H \"Content-Type: application/json\" \\ -d ''{\"input\": {}}'''\n  location: header\n  header: Authorization\n  how_to_obtain: Create an API key in connect.emisso.ai/api-keys and copy the secret that starts with connect_sk_…\nnote: No OAuth2 flows, API keys are the only authentication mechanism described.\ndocs: https://connect.emisso.ai/docs/empezar/primera-llamada\n"
source_yaml_url: https://artifacts.apis.io/emisso-ai/authentication/emisso-ai-authentication.yml
summary_line: 1 scheme
tags:
- Company
- Integration
- Fintech
- Automation
---
