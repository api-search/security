---
api_key_in: []
api_specs:
- filename: morph-labs-openapi.yml
  format: yaml
  label: Morph Apply API
  slug: morph-apply-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/morph-labs/refs/heads/main/openapi/morph-labs-openapi.yml
- filename: morph-labs-openapi.yml
  format: yaml
  label: Morph Embeddings API
  slug: morph-embeddings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/morph-labs/refs/heads/main/openapi/morph-labs-openapi.yml
- filename: morph-labs-openapi.yml
  format: yaml
  label: Morph Rerank API
  slug: morph-rerank-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/morph-labs/refs/heads/main/openapi/morph-labs-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Morph Labs Authentication
name_suffix: Authentication
oauth_flows: []
overview: Morph secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Morph
provider_slug: morph-labs
scheme_count: 1
schemes:
- description: Morph API key supplied as a Bearer token in the Authorization header.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/morph-labs-openapi.yml
  type: http
slug: morph-labs-authentication
source_filename: morph-labs-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/morph-labs-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: Morph API key supplied as a Bearer token in the Authorization header.\n  sources:\n  - openapi/morph-labs-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/morph-labs/refs/heads/main/authentication/morph-labs-authentication.yml
summary_line: http · 1 scheme
tags:
- AI
- Code Editing
- Fast Apply
- Embeddings
- Sandboxes
---
