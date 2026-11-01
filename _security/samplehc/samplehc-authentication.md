---
anonymous_access: false
api_key_in: []
api_specs:
- filename: samplehc-openapi-generated.yml
  format: yaml
  label: Sample API
  slug: samplehc-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/samplehc/openapi/_ae-authored/samplehc-openapi-generated.yml
auth_types: []
description: API requests must be authenticated using an API key passed as a Bearer token in the `Authorization` header.
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Samplehc Authentication
name_suffix: Authentication
oauth_flows: []
overview: Sample declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Sample
provider_slug: samplehc
scheme_count: 1
schemes:
- evidence: API requests must be authenticated using an API key passed as a Bearer token in the `Authorization` header.
  header: Authorization
  how_to_obtain: Create and manage your API keys in the Sample Dashboard.
  location: header
  name: Authorization
  type: http-bearer
slug: samplehc-authentication
source_filename: samplehc-authentication.yml
source_heading: Authentication Profile
source_url: https://docs.samplehc.com/guides/authentication.md
source_yaml: "generated: '2026-10-18'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://docs.samplehc.com/guides/authentication.md\nsources:\n- https://docs.samplehc.com/guides/authentication.md\n- https://docs.samplehc.com/workflows/quickstart.md\ndescription: API requests must be authenticated using an API key passed as a Bearer token in the `Authorization` header.\nschemes:\n- type: http-bearer\n  name: Authorization\n  evidence: API requests must be authenticated using an API key passed as a Bearer token in the `Authorization` header.\n  location: header\n  header: Authorization\n  how_to_obtain: Create and manage your API keys in the Sample Dashboard.\ndocs: https://docs.samplehc.com/guides/authentication.md\n"
source_yaml_url: https://artifacts.apis.io/samplehc/authentication/samplehc-authentication.yml
summary_line: 1 scheme
tags:
- Healthcare
- Artificial Intelligence
- Document Automation
- LLM
- Software-as-a-Service
---
