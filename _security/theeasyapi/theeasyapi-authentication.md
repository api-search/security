---
anonymous_access: false
api_key_in: []
api_specs:
- filename: theeasyapi-openapi-generated.yml
  format: yaml
  label: The Easy API API
  slug: theeasyapi-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/theeasyapi/openapi/_ae-authored/theeasyapi-openapi-generated.yml
auth_types: []
description: Authentication schemes for The Easy API
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Theeasyapi Authentication
name_suffix: Authentication
oauth_flows: []
overview: The Easy API declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: The Easy API
provider_slug: theeasyapi
scheme_count: 1
schemes:
- evidence: API keys can be created in the Account section after you have logged in. These keys will be used to connect to the services which you select. It's a required attribute that should be sent as part of the GET URL, or POST XML request.
  how_to_obtain: API keys can be created in the Account section after you have logged in.
  location: path
  name: api_key
  type: apiKey
slug: theeasyapi-authentication
source_filename: theeasyapi-authentication.yml
source_heading: Authentication Profile
source_url: https://theeasyapi.com/docs
source_yaml: "generated: '2026-10-21'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://theeasyapi.com/docs\nsources:\n- https://theeasyapi.com/docs\ndescription: Authentication schemes for The Easy API\nschemes:\n- type: apiKey\n  name: api_key\n  evidence: API keys can be created in the Account section after you have logged in. These keys will be used to connect to the services which\n    you select. It's a required attribute that should be sent as part of the GET URL, or POST XML request.\n  location: path\n  how_to_obtain: API keys can be created in the Account section after you have logged in.\ndocs: https://theeasyapi.com/docs\n"
source_yaml_url: https://artifacts.apis.io/theeasyapi/authentication/theeasyapi-authentication.yml
summary_line: 1 scheme
tags:
- Data
- Integration
- Developer Tools
- Services
---
