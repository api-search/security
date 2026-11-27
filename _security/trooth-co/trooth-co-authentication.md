---
anonymous_access: false
api_key_in: []
api_specs:
- filename: trooth-co-legal-api-openapi.yml
  format: yaml
  label: Trooth Legal API
  slug: trooth-co-legal-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/trooth-co/openapi/trooth-co-legal-api-openapi.yml
- filename: trooth-co-mobile-api-openapi.yml
  format: yaml
  label: Trooth Mobile API
  slug: trooth-co-mobile-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/trooth-co/openapi/trooth-co-mobile-api-openapi.yml
- filename: trooth-co-network-api-openapi.yml
  format: yaml
  label: Trooth Network API
  slug: trooth-co-network-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/trooth-co/openapi/trooth-co-network-api-openapi.yml
- filename: trooth-co-problems-api-openapi.yml
  format: yaml
  label: Trooth Problems API
  slug: trooth-co-problems-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/trooth-co/openapi/trooth-co-problems-api-openapi.yml
- filename: trooth-co-public-mesh-api-openapi.yml
  format: yaml
  label: Trooth Public Mesh API
  slug: trooth-co-public-mesh-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/trooth-co/openapi/trooth-co-public-mesh-api-openapi.yml
- filename: trooth-co-version-api-openapi.yml
  format: yaml
  label: Trooth Version API
  slug: trooth-co-version-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/trooth-co/openapi/trooth-co-version-api-openapi.yml
auth_types: []
description: Authentication schemes for Trooth API as described on the documentation pages.
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Trooth Authentication
name_suffix: Authentication
oauth_flows: []
overview: Trooth declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Trooth
provider_slug: trooth-co
scheme_count: 2
schemes:
- evidence: 'The proof Send Authorization: DPoP with the token and a new proof in the DPoP header.'
  header: Authorization
  how_to_obtain: Obtained as a session token, scoped token, or OAuth access token depending on the credential type.
  location: header
  name: DPoP token
  type: http-bearer
- evidence: OAuth access token (Model Context Protocol, Agent2Agent). For https://mcp.trooth.co or https://api.trooth.co/a2a/v1.
  header: Authorization
  how_to_obtain: Issued via the Model Context Protocol OAuth flow (details not published).
  location: header
  name: OAuth access token (Model Context Protocol)
  type: http-bearer
slug: trooth-co-authentication
source_filename: trooth-co-authentication.yml
source_heading: Authentication Profile
source_url: https://trooth.co/docs/authentication
source_yaml: "generated: '2026-11-27'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://trooth.co/docs/authentication\nsources:\n- https://trooth.co/docs/authentication\n- https://trooth.co/docs/quickstart\n- https://trooth.co/docs/quickstart.md\ndescription: Authentication schemes for Trooth API as described on the documentation pages.\nschemes:\n- type: http-bearer\n  name: DPoP token\n  evidence: 'The proof Send Authorization: DPoP with the token and a new proof in the DPoP header.'\n  location: header\n  header: Authorization\n  how_to_obtain: Obtained as a session token, scoped token, or OAuth access token depending on the credential type.\n- type: http-bearer\n  name: OAuth access token (Model Context Protocol)\n  evidence: OAuth access token (Model Context Protocol, Agent2Agent). For https://mcp.trooth.co or https://api.trooth.co/a2a/v1.\n  location: header\n  header: Authorization\n  how_to_obtain: Issued via the Model Context Protocol OAuth flow (details\
  \ not published).\nnote: No explicit OAuth flow URLs, scopes, or token/authorize endpoints are provided in the documentation; those fields are left null. 1 extracted\n  row(s) were dropped because their quote was not on the page.\ndocs: https://trooth.co/docs/authentication\n"
source_yaml_url: https://artifacts.apis.io/trooth-co/authentication/trooth-co-authentication.yml
summary_line: 2 schemes
tags:
- Trust
- Infrastructure
- Cybersecurity
- AI
- Data
---
