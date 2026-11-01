---
anonymous_access: false
api_key_in: []
api_specs:
- filename: hardcover-openapi-generated.yml
  format: yaml
  label: Hardcover API
  slug: hardcover-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hardcover/openapi/_ae-authored/hardcover-openapi-generated.yml
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Hardcover Authentication
name_suffix: Authentication
oauth_flows: []
overview: Hardcover declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Hardcover
provider_slug: hardcover
scheme_count: 2
schemes:
- description: Standard OAuth 2.0 Authorization Code flow with PKCE, required for all clients.
  flow: authorizationCode
  pkce: true
  type: oauth2
- description: Device Authorization Grant (RFC8628) for clients without a browser.
  flow: deviceAuthorization
  type: oauth2
slug: hardcover-authentication
source_filename: hardcover-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-28'\nmethod: searched\nsource: https://docs.hardcover.app/api/oauth\nschemes:\n  - type: oauth2\n    flow: authorizationCode\n    pkce: true\n    description: \"Standard OAuth 2.0 Authorization Code flow with PKCE, required for all clients.\"\n  - type: oauth2\n    flow: deviceAuthorization\n    description: \"Device Authorization Grant (RFC8628) for clients without a browser.\"\n"
source_yaml_url: https://artifacts.apis.io/hardcover/authentication/hardcover-authentication.yml
summary_line: 2 schemes
tags:
- Company
- Social
- Book
- Reading
- Community
- API
---
