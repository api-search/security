---
anonymous_access: false
api_key_in: []
api_specs:
- filename: omophub-openapi-generated.yml
  format: yaml
  label: OMOPHub API
  slug: omophub-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/omophub/openapi/_ae-authored/omophub-openapi-generated.yml
auth_types: []
description: Authentication schemes for OMOPHub
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Omophub Authentication
name_suffix: Authentication
oauth_flows: []
overview: OMOPHub declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: OMOPHub
provider_slug: omophub
scheme_count: 1
schemes:
- evidence: 'Include your API key in the Authorization header:'
  header: Authorization
  how_to_obtain: Generate an API key in the OMOPHub dashboard and use it as a Bearer token in the Authorization header.
  location: header
  name: Bearer
  type: http-bearer
slug: omophub-authentication
source_filename: omophub-authentication.yml
source_heading: Authentication Profile
source_url: https://docs.omophub.com/authentication/overview.md
source_yaml: "generated: '2026-10-23'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://docs.omophub.com/authentication/overview.md\nsources:\n- https://docs.omophub.com/authentication/overview.md\n- https://docs.omophub.com/quickstart.md\n- https://docs.omophub.com/ai/onboarding.md\n- https://docs.omophub.com/sdks/python/overview.md\ndescription: Authentication schemes for OMOPHub\nschemes:\n- type: http-bearer\n  name: Bearer\n  evidence: 'Include your API key in the Authorization header:'\n  location: header\n  header: Authorization\n  how_to_obtain: Generate an API key in the OMOPHub dashboard and use it as a Bearer token in the Authorization header.\nnote: No OAuth2 or other authentication methods are documented on the provided pages.\ndocs: https://docs.omophub.com/authentication/overview.md\n"
source_yaml_url: https://artifacts.apis.io/omophub/authentication/omophub-authentication.yml
summary_line: 1 scheme
tags:
- Company
- Healthcare
- Data Integration
- OMOP
- APIs
---
