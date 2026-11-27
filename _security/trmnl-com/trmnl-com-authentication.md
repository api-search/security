---
anonymous_access: false
api_key_in: []
api_specs:
- filename: trmnl-com-openapi-generated.yml
  format: yaml
  label: TRMNL API
  slug: trmnl-com-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/trmnl-com/openapi/_ae-authored/trmnl-com-openapi-generated.yml
auth_types: []
description: Authentication for TRMNL Account API
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: TRMNL Authentication
name_suffix: Authentication
oauth_flows: []
overview: TRMNL declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: TRMNL
provider_slug: trmnl-com
scheme_count: 1
schemes:
- evidence: Send the key in the Authorization header, with Bearer in front of it.
  header: Authorization
  how_to_obtain: Create a new account API key in the TRMNL Developer section (Account > Developer) and copy the generated key.
  location: header
  name: Account API Key
  type: apiKey
slug: trmnl-com-authentication
source_filename: trmnl-com-authentication.yml
source_heading: Authentication Profile
source_url: https://help.trmnl.com/en/articles/11195228-account-api-keys
source_yaml: "generated: '2026-11-27'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://help.trmnl.com/en/articles/11195228-account-api-keys\nsources:\n- https://help.trmnl.com/en/articles/11195228-account-api-keys\n- https://help.trmnl.com/en/articles/12513240-how-to-preload-wifi-credentials\n- https://docs.trmnl.com/go/partners/getting-started\ndescription: Authentication for TRMNL Account API\nschemes:\n- type: apiKey\n  name: Account API Key\n  evidence: Send the key in the Authorization header, with Bearer in front of it.\n  location: header\n  header: Authorization\n  how_to_obtain: Create a new account API key in the TRMNL Developer section (Account > Developer) and copy the generated key.\nnote: 'Legacy keys (starting with user_) use the same Authorization: Bearer header.'\ndocs: https://help.trmnl.com/en/articles/11195228-account-api-keys\n"
source_yaml_url: https://artifacts.apis.io/trmnl-com/authentication/trmnl-com-authentication.yml
summary_line: 1 scheme
tags:
- ePaper
- Dashboard
- Open Source
---
