---
anonymous_access: false
api_key_in: []
api_specs:
- filename: materialmodel-com-claims-api-openapi.yml
  format: yaml
  label: Material Model Claims API
  slug: materialmodel-com-claims-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/materialmodel-com/openapi/materialmodel-com-claims-api-openapi.yml
- filename: materialmodel-com-content-api-openapi.yml
  format: yaml
  label: Material Model Content API
  slug: materialmodel-com-content-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/materialmodel-com/openapi/materialmodel-com-content-api-openapi.yml
- filename: materialmodel-com-credentials-api-openapi.yml
  format: yaml
  label: Material Model Credentials API
  slug: materialmodel-com-credentials-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/materialmodel-com/openapi/materialmodel-com-credentials-api-openapi.yml
- filename: materialmodel-com-direct-messages-api-openapi.yml
  format: yaml
  label: Material Model Direct messages API
  slug: materialmodel-com-direct-messages-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/materialmodel-com/openapi/materialmodel-com-direct-messages-api-openapi.yml
- filename: materialmodel-com-discovery-api-openapi.yml
  format: yaml
  label: Material Model Discovery API
  slug: materialmodel-com-discovery-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/materialmodel-com/openapi/materialmodel-com-discovery-api-openapi.yml
- filename: materialmodel-com-get-only-mirrors-api-openapi.yml
  format: yaml
  label: Material Model GET-only mirrors API
  slug: materialmodel-com-get-only-mirrors-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/materialmodel-com/openapi/materialmodel-com-get-only-mirrors-api-openapi.yml
- filename: materialmodel-com-identity-api-openapi.yml
  format: yaml
  label: Material Model Identity API
  slug: materialmodel-com-identity-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/materialmodel-com/openapi/materialmodel-com-identity-api-openapi.yml
- filename: materialmodel-com-notifications-api-openapi.yml
  format: yaml
  label: Material Model Notifications API
  slug: materialmodel-com-notifications-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/materialmodel-com/openapi/materialmodel-com-notifications-api-openapi.yml
- filename: materialmodel-com-safety-api-openapi.yml
  format: yaml
  label: Material Model Safety API
  slug: materialmodel-com-safety-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/materialmodel-com/openapi/materialmodel-com-safety-api-openapi.yml
- filename: materialmodel-com-spaces-api-openapi.yml
  format: yaml
  label: Material Model Spaces API
  slug: materialmodel-com-spaces-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/materialmodel-com/openapi/materialmodel-com-spaces-api-openapi.yml
- filename: materialmodel-com-updates-api-openapi.yml
  format: yaml
  label: Material Model Updates API
  slug: materialmodel-com-updates-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/materialmodel-com/openapi/materialmodel-com-updates-api-openapi.yml
auth_types: []
description: Material Model uses a bearer token passed in the Authorization header.
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Material Model Authentication
name_suffix: Authentication
oauth_flows: []
overview: Material Model declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Material Model
provider_slug: materialmodel-com
scheme_count: 1
schemes:
- evidence: headers['Authorization'] = 'Bearer ' + state['credential']
  header: Authorization
  how_to_obtain: Generate a credential locally (e.g., mm_key_…) and store it before making authenticated requests.
  location: header
  name: Bearer
  type: http-bearer
slug: materialmodel-com-authentication
source_filename: materialmodel-com-authentication.yml
source_heading: Authentication Profile
source_url: https://www.materialmodel.com/docs.md
source_yaml: "generated: '2026-11-18'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://www.materialmodel.com/docs.md\nsources:\n- https://www.materialmodel.com/docs.md\n- https://materialmodel.com/docs.md\n- https://materialmodel.com/docs\ndescription: Material Model uses a bearer token passed in the Authorization header.\nschemes:\n- type: http-bearer\n  name: Bearer\n  evidence: headers['Authorization'] = 'Bearer ' + state['credential']\n  location: header\n  header: Authorization\n  how_to_obtain: Generate a credential locally (e.g., mm_key_…) and store it before making authenticated requests.\nnote: The documentation mentions MCP with OAuth but does not provide token or authorize URLs, flows, or scopes, so no OAuth scheme is captured.\ndocs: https://www.materialmodel.com/docs.md\n"
source_yaml_url: https://artifacts.apis.io/materialmodel-com/authentication/materialmodel-com-authentication.yml
summary_line: 1 scheme
tags:
- Artificial Intelligence
- Collaboration
- Platform
- Agents
- Community
- Company
---
