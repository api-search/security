---
anonymous_access: false
api_key_in: []
api_specs:
- filename: liblab-howto-openapi-generated.yml
  format: yaml
  label: Liblab howto API
  slug: howto-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/liblab/refs/heads/main/openapi/_ae-authored/liblab-howto-openapi-generated.yml
- filename: liblab-tutorials-openapi-generated.yml
  format: yaml
  label: Liblab tutorials API
  slug: tutorials-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/liblab/refs/heads/main/openapi/_ae-authored/liblab-tutorials-openapi-generated.yml
auth_types: []
description: Authentication methods supported by liblab SDKs and CLI.
kind: authentication
layout: security
mechanism_count: 5
method: searched
name: Liblab Authentication
name_suffix: Authentication
oauth_flows: []
overview: Liblab declares 5 security scheme(s) across its OpenAPI definitions.
provider_name: Liblab
provider_slug: liblab
scheme_count: 5
schemes:
- evidence: By default the X-API-KEY header is used to send the API key
  header: X-API-KEY
  how_to_obtain: Set the API key in the SDK config or via setApiKey method; can be customized in the config file.
  location: header
  name: apikey
  type: apiKey
- evidence: Basic authentication with a user name and password
  how_to_obtain: Provide username and password when configuring the SDK.
  name: basic
  type: http-basic
- evidence: Bearer token authentication
  header: Authorization
  how_to_obtain: Supply the bearer token in the SDK config or via environment variable.
  location: header
  name: bearer
  type: http-bearer
- evidence: Custom access token authentication
  how_to_obtain: Provide the custom token as defined by the API.
  name: custom
  type: other
- evidence: OAuth authentication
  how_to_obtain: Obtain OAuth credentials as described by the API; details not provided on the page.
  name: oauth
  type: oauth2
slug: liblab-authentication
source_filename: liblab-authentication.yml
source_heading: Authentication Profile
source_url: https://liblab.com/docs/concepts/authentication
source_yaml: "generated: '2026-10-04'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://liblab.com/docs/concepts/authentication\nsources:\n- https://liblab.com/docs/concepts/authentication\n- https://liblab.com/docs/cli/cli-overview-auth\n- https://liblab.com/docs/concepts/authentication\n- https://liblab.com/docs/cli/cli-overview-auth\ndescription: Authentication methods supported by liblab SDKs and CLI.\nschemes:\n- type: apiKey\n  name: apikey\n  evidence: By default the X-API-KEY header is used to send the API key\n  location: header\n  header: X-API-KEY\n  how_to_obtain: Set the API key in the SDK config or via setApiKey method; can be customized in the config file.\n- type: http-basic\n  name: basic\n  evidence: Basic authentication with a user name and password\n  how_to_obtain: Provide username and password when configuring the SDK.\n- type: http-bearer\n  name: bearer\n  evidence: Bearer token authentication\n  location: header\n  header: Authorization\n\
  \  how_to_obtain: Supply the bearer token in the SDK config or via environment variable.\n- type: other\n  name: custom\n  evidence: Custom access token authentication\n  how_to_obtain: Provide the custom token as defined by the API.\n- type: oauth2\n  name: oauth\n  evidence: OAuth authentication\n  how_to_obtain: Obtain OAuth credentials as described by the API; details not provided on the page.\ndocs: https://liblab.com/docs/concepts/authentication\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/liblab/refs/heads/main/authentication/liblab-authentication.yml
summary_line: 5 schemes
tags:
- SDK
- SDK Generation
- Code Generation
- OpenAPI
- Developer Tools
- MCP
- AI Agents
- Postman
- Terraform
- Developer Experience
---
