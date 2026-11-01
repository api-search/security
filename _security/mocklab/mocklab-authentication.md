---
anonymous_access: false
api_key_in: []
api_specs:
- filename: mocklab-openapi-generated.yml
  format: yaml
  label: MockLab API
  slug: mocklab-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mocklab/openapi/_ae-authored/mocklab-openapi-generated.yml
auth_types: []
description: Authentication methods supported by MockLab (WireMock) as documented.
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Mocklab Authentication
name_suffix: Authentication
oauth_flows: []
overview: MockLab declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: MockLab
provider_slug: mocklab
scheme_count: 2
schemes:
- evidence: The most common authentication method using a static token in a header.
  header: Authorization
  how_to_obtain: Configured in the local `~/.wiremock/config.yaml` file under the `authenticators` section.
  location: header
  name: header_token
  type: apiKey
- evidence: The WireMock Cloud API uses HTTP Basic authentication, where the username is your username and the password is your API key.
  header: Authorization
  how_to_obtain: API token is found on the WireMock Cloud account security page; the username is the account email.
  location: header
  name: basic
  type: http-basic
slug: mocklab-authentication
source_filename: mocklab-authentication.yml
source_heading: Authentication Profile
source_url: https://docs.wiremock.io/ai-mcp/http-request-authentication.md
source_yaml: "generated: '2026-10-21'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://docs.wiremock.io/ai-mcp/http-request-authentication.md\nsources:\n- https://docs.wiremock.io/ai-mcp/http-request-authentication.md\n- https://docs.wiremock.io/authentication.md\n- https://docs.wiremock.io/response-templating/jwt.md\n- https://docs.wiremock.io/api-reference/security/regenerate-a-users-api-token.md\ndescription: Authentication methods supported by MockLab (WireMock) as documented.\nschemes:\n- type: apiKey\n  name: header_token\n  evidence: The most common authentication method using a static token in a header.\n  location: header\n  header: Authorization\n  how_to_obtain: Configured in the local `~/.wiremock/config.yaml` file under the `authenticators` section.\n- type: http-basic\n  name: basic\n  evidence: The WireMock Cloud API uses HTTP Basic authentication, where the username is your username and the password is your API key.\n  location: header\n  header:\
  \ Authorization\n  how_to_obtain: API token is found on the WireMock Cloud account security page; the username is the account email.\nnote: No OAuth2 flows are documented on the provided pages. 1 extracted row(s) were dropped because their quote was not on the page.\ndocs: https://docs.wiremock.io/ai-mcp/http-request-authentication.md\n"
source_yaml_url: https://artifacts.apis.io/mocklab/authentication/mocklab-authentication.yml
summary_line: 2 schemes
tags:
- API Mocking
- Environment Simulation
- Testing
- Fintech
- Service Virtualization
- Cloud Service
---
