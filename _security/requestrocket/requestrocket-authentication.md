---
anonymous_access: false
api_key_in: []
api_specs:
- filename: requestrocket-requestrocket-api-api-openapi.yml
  format: yaml
  label: RequestRocket API
  slug: requestrocket-api-2
  spec_type: OpenAPI
  url: https://artifacts.apis.io/requestrocket/openapi/requestrocket-requestrocket-api-api-openapi.yml
- filename: requestrocket-openapi-generated.yml
  format: yaml
  label: RequestRocket API
  slug: requestrocket-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/requestrocket/openapi/_ae-authored/requestrocket-openapi-generated.yml
auth_types: []
description: Core API uses personal user tokens placed in the Authorization header without a Bearer prefix.
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Requestrocket Authentication
name_suffix: Authentication
oauth_flows: []
overview: RequestRocket declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: RequestRocket
provider_slug: requestrocket
scheme_count: 1
schemes:
- evidence: 'Include your user token in the Authorization header of every Core API request:'
  header: Authorization
  how_to_obtain: Navigate to Settings → Keys tab and copy the personal user token displayed.
  location: header
  name: User Token
  type: other
slug: requestrocket-authentication
source_filename: requestrocket-authentication.yml
source_heading: Authentication Profile
source_url: https://docs.requestrocket.com/docs/api-reference/core-api/authentication
source_yaml: "generated: '2026-10-18'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://docs.requestrocket.com/docs/api-reference/core-api/authentication\nsources:\n- https://docs.requestrocket.com/docs/api-reference/core-api/authentication\n- https://docs.requestrocket.com/docs/guides/personal-settings\n- https://docs.requestrocket.com/docs/guides/credentials\n- https://docs.requestrocket.com/docs/api-reference/core-api/credentials\ndescription: Core API uses personal user tokens placed in the Authorization header without a Bearer prefix.\nschemes:\n- type: other\n  name: User Token\n  evidence: 'Include your user token in the Authorization header of every Core API request:'\n  location: header\n  header: Authorization\n  how_to_obtain: Navigate to Settings → Keys tab and copy the personal user token displayed.\ndocs: https://docs.requestrocket.com/docs/api-reference/core-api/authentication\n"
source_yaml_url: https://artifacts.apis.io/requestrocket/authentication/requestrocket-authentication.yml
summary_line: 1 scheme
tags:
- Company
- Artificial Intelligence
- Security
- Software-as-a-Service
- Access Control
---
