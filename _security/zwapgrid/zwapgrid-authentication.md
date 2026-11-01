---
anonymous_access: false
api_key_in: []
api_specs:
- filename: zwapgrid-openapi-generated.yml
  format: yaml
  label: Zwapgrid API
  slug: zwapgrid-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/zwapgrid/openapi/_ae-authored/zwapgrid-openapi-generated.yml
auth_types: []
description: Authentication for Zwapgrid APIs uses API Keys passed in a custom header.
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Zwapgrid Authentication
name_suffix: Authentication
oauth_flows: []
overview: Zwapgrid declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Zwapgrid
provider_slug: zwapgrid
scheme_count: 1
schemes:
- evidence: 'When you call API.1, pass your API Key in every request using the `x-api-key` HTTP header:'
  header: x-api-key
  how_to_obtain: Create an API Key in the Client Portal per environment.
  location: header
  name: API Key
  type: apiKey
slug: zwapgrid-authentication
source_filename: zwapgrid-authentication.yml
source_heading: Authentication Profile
source_url: https://docs.zwapgrid.com/client-portal/api-keys.md
source_yaml: "generated: '2026-10-19'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://docs.zwapgrid.com/client-portal/api-keys.md\nsources:\n- https://docs.zwapgrid.com/client-portal/api-keys.md\n- https://docs.zwapgrid.com/client-portal/api-keys/usage.md\n- https://docs.zwapgrid.com/client-portal/api-keys/security.md\n- https://docs.zwapgrid.com/client-portal/api-keys/api-key-lifecycle.md\ndescription: Authentication for Zwapgrid APIs uses API Keys passed in a custom header.\nschemes:\n- type: apiKey\n  name: API Key\n  evidence: 'When you call API.1, pass your API Key in every request using the `x-api-key` HTTP header:'\n  location: header\n  header: x-api-key\n  how_to_obtain: Create an API Key in the Client Portal per environment.\nnote: No OAuth2, HTTP bearer, or other authentication schemes are documented on the provided pages.\ndocs: https://docs.zwapgrid.com/client-portal/api-keys.md\n"
source_yaml_url: https://artifacts.apis.io/zwapgrid/authentication/zwapgrid-authentication.yml
summary_line: 1 scheme
tags:
- Accounting
- Fintech
- Integration
- Software-as-a-Service
---
