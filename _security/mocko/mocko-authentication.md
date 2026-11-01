---
anonymous_access: false
api_key_in: []
api_specs:
- filename: mocko-mocko-api-api-openapi.yml
  format: yaml
  label: Mocko API
  slug: mocko-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mocko/openapi/mocko-mocko-api-api-openapi.yml
- filename: mocko-core-openapi-generated.yml
  format: yaml
  label: Mocko core API
  slug: core-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mocko/openapi/_ae-authored/mocko-core-openapi-generated.yml
- filename: mocko-creating-mocks-openapi-generated.yml
  format: yaml
  label: Mocko creating mocks API
  slug: creating-mocks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mocko/openapi/_ae-authored/mocko-creating-mocks-openapi-generated.yml
- filename: mocko-recipes-openapi-generated.yml
  format: yaml
  label: Mocko Recipes Overview API
  slug: recipes-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mocko/openapi/_ae-authored/mocko-recipes-openapi-generated.yml
- filename: mocko-v1-openapi-generated.yml
  format: yaml
  label: Mocko Legacy v1 docs API
  slug: v1-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mocko/openapi/_ae-authored/mocko-v1-openapi-generated.yml
auth_types: []
description: Mocko uses a bearer token for authentication when the mock server is configured with MANAGEMENT_AUTH_MODE=all.
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Mocko Authentication
name_suffix: Authentication
oauth_flows: []
overview: Mocko declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Mocko
provider_slug: mocko
scheme_count: 1
schemes:
- evidence: 'It is sent as Authorization: Bearer <secret> on every request'
  header: Authorization
  how_to_obtain: Read the deploy secret from the server configuration (DEPLOY_SECRET) or from the Helm chart release secret.
  location: header
  name: Bearer
  type: http-bearer
slug: mocko-authentication
source_filename: mocko-authentication.yml
source_heading: Authentication Profile
source_url: https://mocko.dev/docs/sdk/auth
source_yaml: "generated: '2026-10-21'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://mocko.dev/docs/sdk/auth\nsources:\n- https://mocko.dev/docs/sdk/auth\n- https://mocko.dev/docs/getting-started\n- https://mocko.dev/docs/sdk/getting-started\n- https://mocko.dev/docs/cloud/getting-started\ndescription: Mocko uses a bearer token for authentication when the mock server is configured with MANAGEMENT_AUTH_MODE=all.\nschemes:\n- type: http-bearer\n  name: Bearer\n  evidence: 'It is sent as Authorization: Bearer <secret> on every request'\n  location: header\n  header: Authorization\n  how_to_obtain: Read the deploy secret from the server configuration (DEPLOY_SECRET) or from the Helm chart release secret.\ndocs: https://mocko.dev/docs/sdk/auth\n"
source_yaml_url: https://artifacts.apis.io/mocko/authentication/mocko-authentication.yml
summary_line: 1 scheme
tags:
- Company
- API Mocking
- Development Tools
- Testing
- Collaboration
---
