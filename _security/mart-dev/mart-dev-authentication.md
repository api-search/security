---
anonymous_access: false
api_key_in: []
api_specs:
- filename: mart-dev-linked-in-api-openapi.yml
  format: yaml
  label: Mart.dev Linked In API
  slug: mart-dev-linked-in-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mart-dev/refs/heads/main/openapi/mart-dev-linked-in-api-openapi.yml
auth_types: []
description: Pass your API key in the header
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Mart Dev Authentication
name_suffix: Authentication
oauth_flows: []
overview: Mart.dev declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Mart.dev
provider_slug: mart-dev
scheme_count: 1
schemes:
- evidence: Every request uses the x-api-key header. You can get a key in API Keys.
  header: x-api-key
  how_to_obtain: Get a key in API Keys (default key or create additional keys).
  location: header
  name: x-api-key
  type: apiKey
slug: mart-dev-authentication
source_filename: mart-dev-authentication.yml
source_heading: Authentication Profile
source_url: https://mart.dev/docs/#authentication
source_yaml: "generated: '2026-09-28'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://mart.dev/docs/#authentication\nsources:\n- https://mart.dev/docs/#authentication\n- https://mart.dev/docs/\n- https://mart.dev/docs/#quickstart\ndescription: Pass your API key in the header\nschemes:\n- type: apiKey\n  name: x-api-key\n  evidence: Every request uses the x-api-key header. You can get a key in API Keys.\n  location: header\n  header: x-api-key\n  how_to_obtain: Get a key in API Keys (default key or create additional keys).\ndocs: https://mart.dev/docs/#authentication\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mart-dev/refs/heads/main/authentication/mart-dev-authentication.yml
summary_line: 1 scheme
tags:
- Company
- Data
- LinkedIn
- Unofficial
---
