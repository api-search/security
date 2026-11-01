---
anonymous_access: false
api_key_in: []
api_specs:
- filename: qardapi-openapi-generated.yml
  format: yaml
  label: Qard API
  slug: qardapi-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/qardapi/openapi/_ae-authored/qardapi-openapi-generated.yml
auth_types: []
description: Authentication methods for Qard API
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Qardapi Authentication
name_suffix: Authentication
oauth_flows: []
overview: Qard declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Qard
provider_slug: qardapi
scheme_count: 2
schemes:
- evidence: To use the API with the Api Key authentication method you have to include the header X-API-KEY in every request.
  header: X-API-KEY
  location: header
  name: X-API-KEY
  type: apiKey
- evidence: OAuth2.0 implicit is the preferred way if you want to build an application which make api calls directly from a browser.
  name: OAuth2.0 implicit
  type: oauth2
slug: qardapi-authentication
source_filename: qardapi-authentication.yml
source_heading: Authentication Profile
source_url: https://developers.qardapi.com/api-basics/authentication/
source_yaml: "generated: '2026-10-21'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://developers.qardapi.com/api-basics/authentication/\nsources:\n- https://developers.qardapi.com/api-basics/authentication/\ndescription: Authentication methods for Qard API\nschemes:\n- type: apiKey\n  name: X-API-KEY\n  evidence: To use the API with the Api Key authentication method you have to include the header X-API-KEY in every request.\n  location: header\n  header: X-API-KEY\n- type: oauth2\n  name: OAuth2.0 implicit\n  evidence: OAuth2.0 implicit is the preferred way if you want to build an application which make api calls directly from a browser.\ndocs: https://developers.qardapi.com/api-basics/authentication/\n"
source_yaml_url: https://artifacts.apis.io/qardapi/authentication/qardapi-authentication.yml
summary_line: 2 schemes
tags:
- Company
---
