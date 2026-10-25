---
anonymous_access: false
api_key_in: []
api_specs:
- filename: keysight-technologies-openapi-generated.yml
  format: yaml
  label: Keysight Technologies API
  slug: keysight-technologies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/keysight-technologies/refs/heads/main/openapi/_ae-authored/keysight-technologies-openapi-generated.yml
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Keysight Technologies Authentication
name_suffix: Authentication
oauth_flows: []
overview: Keysight Technologies declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Keysight Technologies
provider_slug: keysight-technologies
scheme_count: 1
schemes:
- authorizationUrl: /auth/realms/keysight/protocol/openid-connect/auth
  flow: authorizationCode / refresh token (OpenID Connect via Keycloak)
  note: Relative to the customer controller host; SDK examples use an offline refresh token from the CyPerf UI (OFFLINE_TOKEN_FROM_CYPERF_UI).
  scopes:
  - offline_access
  - openid
  type: oauth2
slug: keysight-technologies-authentication
source_filename: keysight-technologies-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "name: Keysight CyPerf authentication\ngenerated: '2026-10-19'\nmethod: searched\nsource: https://github.com/Keysight/cyperf-api-wrapper/blob/main/README.md\ndocs: https://github.com/Keysight/cyperf-api-wrapper/blob/main/README.md#documentation-for-authorization\nschemes:\n- type: oauth2\n  flow: authorizationCode / refresh token (OpenID Connect via Keycloak)\n  authorizationUrl: /auth/realms/keysight/protocol/openid-connect/auth\n  scopes:\n  - offline_access\n  - openid\n  note: Relative to the customer controller host; SDK examples use an offline refresh token from the CyPerf UI (OFFLINE_TOKEN_FROM_CYPERF_UI).\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/keysight-technologies/refs/heads/main/authentication/keysight-technologies-authentication.yml
summary_line: 1 scheme
tags:
- Network Testing
- Test and Measurement
- Performance Testing
- Security Testing
- Electronics
- Traffic Generation
- MCP
---
