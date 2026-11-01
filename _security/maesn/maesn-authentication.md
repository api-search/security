---
anonymous_access: false
api_key_in: []
api_specs:
- filename: maesn-accounting-api-openapi.yml
  format: yaml
  label: Maesn Accounting API
  slug: maesn-accounting-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/maesn/openapi/maesn-accounting-api-openapi.yml
- filename: maesn-auth-api-openapi.yml
  format: yaml
  label: Maesn Auth API
  slug: maesn-auth-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/maesn/openapi/maesn-auth-api-openapi.yml
- filename: maesn-tenants-api-openapi.yml
  format: yaml
  label: Maesn Tenants API
  slug: maesn-tenants-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/maesn/openapi/maesn-tenants-api-openapi.yml
- filename: maesn-user-api-openapi.yml
  format: yaml
  label: Maesn User API
  slug: maesn-user-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/maesn/openapi/maesn-user-api-openapi.yml
- filename: maesn-webhook-api-openapi.yml
  format: yaml
  label: Maesn Webhook API
  slug: maesn-webhook-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/maesn/openapi/maesn-webhook-api-openapi.yml
auth_types: []
description: Authentication schemes for Maesn Unified API
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Maesn Authentication
name_suffix: Authentication
oauth_flows: []
overview: Maesn declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Maesn
provider_slug: maesn
scheme_count: 2
schemes:
- evidence: For any request you make into the maesn API this is the header that authenticates yourself as a user of the maesn API.
  header: X-API-KEY
  how_to_obtain: Contact via the link https://www.maesn.com/contact/ to get an API key.
  location: header
  name: X-API-KEY
  type: apiKey
- evidence: When trying to access your end user's information in the target system, you will only be allowed to do so, if the end user went through the registration flow and authenticated to the target system, and you stored the `X-ACCOUNT-KEY` to use with these requests.
  header: X-ACCOUNT-KEY
  how_to_obtain: Obtained after the end user completes the authentication flow and an account token is returned.
  location: header
  name: X-ACCOUNT-KEY
  type: apiKey
slug: maesn-authentication
source_filename: maesn-authentication.yml
source_heading: Authentication Profile
source_url: https://docs.maesn.com/authentication.md
source_yaml: "generated: '2026-10-20'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://docs.maesn.com/authentication.md\nsources:\n- https://docs.maesn.com/authentication.md\n- https://docs.maesn.com/api-reference/auth/get-auth.md\n- https://docs.maesn.com/api-reference/auth/post-auth.md\n- https://docs.maesn.com/api-reference/auth/get-environments.md\ndescription: Authentication schemes for Maesn Unified API\nschemes:\n- type: apiKey\n  name: X-API-KEY\n  evidence: For any request you make into the maesn API this is the header that authenticates yourself as a user of the maesn API.\n  location: header\n  header: X-API-KEY\n  how_to_obtain: Contact via the link https://www.maesn.com/contact/ to get an API key.\n- type: apiKey\n  name: X-ACCOUNT-KEY\n  evidence: When trying to access your end user's information in the target system, you will only be allowed to do so, if the end user went through\n    the registration flow and authenticated to the target system,\
  \ and you stored the `X-ACCOUNT-KEY` to use with these requests.\n  location: header\n  header: X-ACCOUNT-KEY\n  how_to_obtain: Obtained after the end user completes the authentication flow and an account token is returned.\ndocs: https://docs.maesn.com/authentication.md\n"
source_yaml_url: https://artifacts.apis.io/maesn/authentication/maesn-authentication.yml
summary_line: 2 schemes
tags:
- ERP
- Accounting
- Integration
- Software-as-a-Service
---
