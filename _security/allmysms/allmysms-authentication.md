---
anonymous_access: false
api_key_in: []
api_specs:
- filename: allmysms-openapi-generated.yml
  format: yaml
  label: All My SMS API
  slug: allmysms-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/allmysms/openapi/_ae-authored/allmysms-openapi-generated.yml
auth_types: []
description: Authentication
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: All My SMS Authentication
name_suffix: Authentication
oauth_flows: []
overview: All My SMS declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: All My SMS
provider_slug: allmysms
scheme_count: 1
schemes:
- evidence: API services use the Basic authentication method to identify users.
  header: Authorization
  how_to_obtain: The API key (apiKey) can be retrieved by logging in the customer area (section API / Api Key & Parameters) and combined with the login to form the AUTH_TOKEN.
  location: header
  name: Basic
  type: http-basic
slug: allmysms-authentication
source_filename: allmysms-authentication.yml
source_heading: Authentication Profile
source_url: https://doc.allmysms.com/api/fr/
source_yaml: "generated: '2026-11-16'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://doc.allmysms.com/api/fr/\nsources:\n- https://doc.allmysms.com/api/fr/\n- https://doc.allmysms.com/api/en/\ndescription: Authentication\nschemes:\n- type: http-basic\n  name: Basic\n  evidence: API services use the Basic authentication method to identify users.\n  location: header\n  header: Authorization\n  how_to_obtain: The API key (apiKey) can be retrieved by logging in the customer area (section API / Api Key & Parameters) and combined with\n    the login to form the AUTH_TOKEN.\ndocs: https://doc.allmysms.com/api/fr/\n"
source_yaml_url: https://artifacts.apis.io/allmysms/authentication/allmysms-authentication.yml
summary_line: 1 scheme
tags:
- Company
- SMS
- Marketing
- Communications
---
