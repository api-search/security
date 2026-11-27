---
anonymous_access: false
api_key_in: []
api_specs:
- filename: myself-md-blog-api-openapi.yml
  format: yaml
  label: myself.md Blog API
  slug: myself-md-blog-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/myself-md/openapi/myself-md-blog-api-openapi.yml
- filename: myself-md-dataset-catalog-api-openapi.yml
  format: yaml
  label: myself.md Dataset Catalog API
  slug: myself-md-dataset-catalog-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/myself-md/openapi/myself-md-dataset-catalog-api-openapi.yml
- filename: myself-md-queries-api-openapi.yml
  format: yaml
  label: myself.md Queries API
  slug: myself-md-queries-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/myself-md/openapi/myself-md-queries-api-openapi.yml
auth_types: []
description: Authentication methods published for myself.md
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: myself.md Authentication
name_suffix: Authentication
oauth_flows: []
overview: myself.md declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: myself.md
provider_slug: myself-md
scheme_count: 1
schemes:
- evidence: Sign in when your assistant opens the connection flow.
  header: Authorization
  how_to_obtain: Sign in when your assistant opens the connection flow.
  location: header
  name: Bearer
  type: http-bearer
slug: myself-md-authentication
source_filename: myself-md-authentication.yml
source_heading: Authentication Profile
source_url: https://myself.md/docs
source_yaml: "generated: '2026-11-18'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://myself.md/docs\nsources:\n- https://myself.md/docs\n- https://myself.md/.well-known/oauth-protected-resource/mcp\n- https://github.com/CodyBontecou/myself.md#run-locally\n- https://myself.md/v1/docs\ndescription: Authentication methods published for myself.md\nschemes:\n- type: http-bearer\n  name: Bearer\n  evidence: Sign in when your assistant opens the connection flow.\n  location: header\n  header: Authorization\n  how_to_obtain: Sign in when your assistant opens the connection flow.\ndocs: https://myself.md/docs\n"
source_yaml_url: https://artifacts.apis.io/myself-md/authentication/myself-md-authentication.yml
summary_line: 1 scheme
tags:
- Health
- Personal Data
- Mobile App
- Open Source
- AI Integration
---
