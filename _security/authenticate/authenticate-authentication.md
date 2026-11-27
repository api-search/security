---
anonymous_access: false
api_key_in: []
api_specs:
- filename: authenticate-methods-api-openapi.yml
  format: yaml
  label: Authenticate Methods API
  slug: authenticate-methods-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/authenticate/openapi/authenticate-methods-api-openapi.yml
- filename: authenticate-mock-apis-api-openapi.yml
  format: yaml
  label: Authenticate Mock APIs API
  slug: authenticate-mock-apis-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/authenticate/openapi/authenticate-mock-apis-api-openapi.yml
- filename: authenticate-webhooks-api-openapi.yml
  format: yaml
  label: Authenticate Webhooks API
  slug: authenticate-webhooks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/authenticate/openapi/authenticate-webhooks-api-openapi.yml
auth_types: []
description: Authentication schemes for Authenticate
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Authenticate Authentication
name_suffix: Authentication
oauth_flows: []
overview: Authenticate declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Authenticate
provider_slug: authenticate
scheme_count: 1
schemes:
- evidence: It must be included in the Authorization header as a Bearer token.
  header: Authorization
  how_to_obtain: Log in to your Authenticate® account, navigate to Settings, reveal the API Key, and copy it.
  location: header
  name: API Key
  type: http-bearer
slug: authenticate-authentication
source_filename: authenticate-authentication.yml
source_heading: Authentication Profile
source_url: https://docs.authenticate.com/docs/api-key.md
source_yaml: "generated: '2026-11-09'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://docs.authenticate.com/docs/api-key.md\nsources:\n- https://docs.authenticate.com/docs/api-key.md\n- https://docs.authenticate.com/reference/multi-factor-authentication.md\n- https://docs.authenticate.com/reference/multi-factor-authentication\n- https://docs.authenticate.com/docs/api-key\ndescription: Authentication schemes for Authenticate\nschemes:\n- type: http-bearer\n  name: API Key\n  evidence: It must be included in the Authorization header as a Bearer token.\n  location: header\n  header: Authorization\n  how_to_obtain: Log in to your Authenticate® account, navigate to Settings, reveal the API Key, and copy it.\nnote: No OAuth2 or other authentication schemes are documented on the provided pages.\ndocs: https://docs.authenticate.com/docs/api-key.md\n"
source_yaml_url: https://artifacts.apis.io/authenticate/authentication/authenticate-authentication.yml
summary_line: 1 scheme
tags:
- Company
- Identity Verification
- KBA
- Background Checks
---
