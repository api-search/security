---
anonymous_access: false
api_key_in: []
api_specs:
- filename: kasar-app-openapi-generated.yml
  format: yaml
  label: Kasar API
  slug: kasar-app-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/kasar-app/openapi/_ae-authored/kasar-app-openapi-generated.yml
auth_types: []
description: Authentication is performed by sending the integration key as a Bearer token in the Authorization header.
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Kasar Authentication
name_suffix: Authentication
oauth_flows: []
overview: Kasar declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Kasar
provider_slug: kasar-app
scheme_count: 1
schemes:
- evidence: 'Send them as a bearer token: curl https://platform.kasar.app/api/v1/objects \ -H "Authorization: Bearer ksr_svc_eyJhbGciOiJIUzI1NiJ9..."'
  header: Authorization
  how_to_obtain: Create an integration in Settings → API and webhooks, give it a name, set rights and expiration, then copy the displayed key (starts with ksr_svc_).
  location: header
  name: Bearer
  type: http-bearer
slug: kasar-app-authentication
source_filename: kasar-app-authentication.yml
source_heading: Authentication Profile
source_url: https://docs.kasar.app/docs/api-reference/authentication
source_yaml: "generated: '2026-11-13'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://docs.kasar.app/docs/api-reference/authentication\nsources:\n- https://docs.kasar.app/docs/api-reference/authentication\n- https://docs.kasar.app/docs/api-reference\n- https://docs.kasar.app/docs/mcp/setup\ndescription: Authentication is performed by sending the integration key as a Bearer token in the Authorization header.\nschemes:\n- type: http-bearer\n  name: Bearer\n  evidence: 'Send them as a bearer token: curl https://platform.kasar.app/api/v1/objects \\ -H \"Authorization: Bearer ksr_svc_eyJhbGciOiJIUzI1NiJ9...\"'\n  location: header\n  header: Authorization\n  how_to_obtain: Create an integration in Settings → API and webhooks, give it a name, set rights and expiration, then copy the displayed key\n    (starts with ksr_svc_).\nnote: No OAuth2, apiKey, or other authentication schemes are documented.\ndocs: https://docs.kasar.app/docs/api-reference/authentication\n"
source_yaml_url: https://artifacts.apis.io/kasar-app/authentication/kasar-app-authentication.yml
summary_line: 1 scheme
tags:
- CRM
- AI-native
- Sales
- Automation
- Software-as-a-Service
---
