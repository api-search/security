---
anonymous_access: false
api_key_in: []
api_specs:
- filename: hermai-brand-api-openapi.yml
  format: yaml
  label: Hermai Brand API
  slug: hermai-brand-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hermai/openapi/hermai-brand-api-openapi.yml
- filename: hermai-api-openapi.json
  format: json
  label: Hermai Agent-Native API API
  slug: hermai-agent-native-api-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hermai/openapi/_original/hermai-api-openapi.json
auth_types: []
description: Hermai Brand API uses an API key sent as a Bearer token in the Authorization header.
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Hermai Authentication
name_suffix: Authentication
oauth_flows: []
overview: Hermai Brand API declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Hermai Brand API
provider_slug: hermai
scheme_count: 1
schemes:
- evidence: '-H "Authorization: Bearer ${ HERMAI_API_KEY }"'
  header: Authorization
  how_to_obtain: Create an API key in Dashboard > API Keys and copy it.
  location: header
  name: Authorization
  type: http-bearer
slug: hermai-authentication
source_filename: hermai-authentication.yml
source_heading: Authentication Profile
source_url: https://docs.hermai.ai/quickstart
source_yaml: "generated: '2026-10-18'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://docs.hermai.ai/quickstart\nsources:\n- https://docs.hermai.ai/quickstart\ndescription: Hermai Brand API uses an API key sent as a Bearer token in the Authorization header.\nschemes:\n- type: http-bearer\n  name: Authorization\n  evidence: '-H \"Authorization: Bearer ${ HERMAI_API_KEY }\"'\n  location: header\n  header: Authorization\n  how_to_obtain: Create an API key in Dashboard > API Keys and copy it.\ndocs: https://docs.hermai.ai/quickstart\n"
source_yaml_url: https://artifacts.apis.io/hermai/authentication/hermai-authentication.yml
summary_line: 1 scheme
tags:
- Company
- Branding
- Marketing
- Software-as-a-Service
---
