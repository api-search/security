---
anonymous_access: false
api_key_in: []
api_specs:
- filename: subq-openapi-generated.yml
  format: yaml
  label: Subquadratic API
  slug: subq-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/subq/openapi/_ae-authored/subq-openapi-generated.yml
auth_types: []
description: Every API request requires an API key in the `Authorization` header using the Bearer scheme.
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Subq Authentication
name_suffix: Authentication
oauth_flows: []
overview: Subquadratic declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Subquadratic
provider_slug: subq
scheme_count: 1
schemes:
- evidence: Every API request requires an API key in the `Authorization` header using the Bearer scheme.
  header: Authorization
  how_to_obtain: Generate a key from console.subq.ai, store it outside your source tree, and send it with each request.
  location: header
  name: Bearer
  type: http-bearer
slug: subq-authentication
source_filename: subq-authentication.yml
source_heading: Authentication Profile
source_url: https://docs.subq.ai/markdown/using-the-api/authentication.md
source_yaml: "generated: '2026-10-19'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://docs.subq.ai/markdown/using-the-api/authentication.md\nsources:\n- https://docs.subq.ai/markdown/using-the-api/authentication.md\n- https://docs.subq.ai/using-the-api/authentication/\n- https://docs.subq.ai/markdown/index.md\n- https://docs.subq.ai/\ndescription: Every API request requires an API key in the `Authorization` header using the Bearer scheme.\nschemes:\n- type: http-bearer\n  name: Bearer\n  evidence: Every API request requires an API key in the `Authorization` header using the Bearer scheme.\n  location: header\n  header: Authorization\n  how_to_obtain: Generate a key from console.subq.ai, store it outside your source tree, and send it with each request.\ndocs: https://docs.subq.ai/markdown/using-the-api/authentication.md\n"
source_yaml_url: https://artifacts.apis.io/subq/authentication/subq-authentication.yml
summary_line: 1 scheme
tags:
- Company
- Artificial Intelligence
- Enterprise
- Decision Models
- Long Context
---
