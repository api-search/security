---
anonymous_access: false
api_key_in: []
api_specs:
- filename: cleanslice-org-openapi-generated.yml
  format: yaml
  label: CleanSlice API
  slug: cleanslice-org-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cleanslice-org/openapi/_ae-authored/cleanslice-org-openapi-generated.yml
auth_types: []
description: Client authenticates using a JWT Bearer token sent in the Authorization header.
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: CleanSlice Authentication
name_suffix: Authentication
oauth_flows: []
overview: CleanSlice declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: CleanSlice
provider_slug: cleanslice-org
scheme_count: 1
schemes:
- evidence: 'addBearerAuth ( { description: ''JWT Bearer token'' , name: ''Authorization'' , bearerFormat: ''Bearer'' , scheme: ''Bearer'' , type: ''http'' , in: ''Header'' } )'
  header: Authorization
  location: header
  name: defaultBearerAuth
  type: http-bearer
slug: cleanslice-org-authentication
source_filename: cleanslice-org-authentication.yml
source_heading: Authentication Profile
source_url: https://cleanslice.org/backend/getting-started.html
source_yaml: "generated: '2026-11-04'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://cleanslice.org/backend/getting-started.html\nsources:\n- https://cleanslice.org/backend/getting-started.html\n- https://cleanslice.org/frontend/getting-started.html\ndescription: Client authenticates using a JWT Bearer token sent in the Authorization header.\nschemes:\n- type: http-bearer\n  name: defaultBearerAuth\n  evidence: 'addBearerAuth ( { description: ''JWT Bearer token'' , name: ''Authorization'' , bearerFormat: ''Bearer'' , scheme: ''Bearer'' , type:\n    ''http'' , in: ''Header'' } )'\n  location: header\n  header: Authorization\ndocs: https://cleanslice.org/backend/getting-started.html\n"
source_yaml_url: https://artifacts.apis.io/cleanslice-org/authentication/cleanslice-org-authentication.yml
summary_line: 1 scheme
tags:
- Architecture
- Full‑Stack Framework
- NestJS
- Nuxt
- AI Agents
- Deployment Platform
- TypeScript
---
