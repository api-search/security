---
anonymous_access: false
api_key_in: []
api_specs:
- filename: inkseal-net-account-api-openapi.yml
  format: yaml
  label: InkSeal Account API
  slug: inkseal-net-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/inkseal-net/openapi/inkseal-net-account-api-openapi.yml
- filename: inkseal-net-credentials-api-openapi.yml
  format: yaml
  label: InkSeal Credentials API
  slug: inkseal-net-credentials-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/inkseal-net/openapi/inkseal-net-credentials-api-openapi.yml
- filename: inkseal-net-credits-api-openapi.yml
  format: yaml
  label: InkSeal Credits API
  slug: inkseal-net-credits-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/inkseal-net/openapi/inkseal-net-credits-api-openapi.yml
- filename: inkseal-net-detection-api-openapi.yml
  format: yaml
  label: InkSeal Detection API
  slug: inkseal-net-detection-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/inkseal-net/openapi/inkseal-net-detection-api-openapi.yml
- filename: inkseal-net-documents-api-openapi.yml
  format: yaml
  label: InkSeal Documents API
  slug: inkseal-net-documents-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/inkseal-net/openapi/inkseal-net-documents-api-openapi.yml
- filename: inkseal-net-envelopes-api-openapi.yml
  format: yaml
  label: InkSeal Envelopes API
  slug: inkseal-net-envelopes-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/inkseal-net/openapi/inkseal-net-envelopes-api-openapi.yml
- filename: inkseal-net-inbound-requests-api-openapi.yml
  format: yaml
  label: InkSeal Inbound Requests API
  slug: inkseal-net-inbound-requests-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/inkseal-net/openapi/inkseal-net-inbound-requests-api-openapi.yml
- filename: inkseal-net-public-links-api-openapi.yml
  format: yaml
  label: InkSeal Public links API
  slug: inkseal-net-public-links-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/inkseal-net/openapi/inkseal-net-public-links-api-openapi.yml
- filename: inkseal-net-templates-api-openapi.yml
  format: yaml
  label: InkSeal Templates API
  slug: inkseal-net-templates-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/inkseal-net/openapi/inkseal-net-templates-api-openapi.yml
- filename: inkseal-net-webhooks-api-openapi.yml
  format: yaml
  label: InkSeal Webhooks API
  slug: inkseal-net-webhooks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/inkseal-net/openapi/inkseal-net-webhooks-api-openapi.yml
auth_types: []
description: Authentication schemes for InkSeal as described in the provided documentation.
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: InkSeal Authentication
name_suffix: Authentication
oauth_flows: []
overview: InkSeal declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: InkSeal
provider_slug: inkseal-net
scheme_count: 2
schemes:
- evidence: Mint a key in Settings, service credentials and send it as a bearer token on every request.
  header: Authorization
  how_to_obtain: Mint a key in Settings, service credentials and send it as a bearer token on every request.
  location: header
  name: Bearer token
  type: http-bearer
- evidence: The client discovers that https://inkseal.net/mcp is an OAuth protected resource and finds our authorization server.
  how_to_obtain: The client discovers that https://inkseal.net/mcp is an OAuth protected resource and finds our authorization server.
  name: OAuth 2.1
  type: oauth2
slug: inkseal-net-authentication
source_filename: inkseal-net-authentication.yml
source_heading: Authentication Profile
source_url: https://inkseal.net/docs/agents/oauth.md
source_yaml: "generated: '2026-11-12'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://inkseal.net/docs/agents/oauth.md\nsources:\n- https://inkseal.net/docs/agents/oauth.md\n- https://inkseal.net/docs/agents/oauth\n- https://inkseal.net/docs/mcp\ndescription: Authentication schemes for InkSeal as described in the provided documentation.\nschemes:\n- type: http-bearer\n  name: Bearer token\n  evidence: Mint a key in Settings, service credentials and send it as a bearer token on every request.\n  location: header\n  header: Authorization\n  how_to_obtain: Mint a key in Settings, service credentials and send it as a bearer token on every request.\n- type: oauth2\n  name: OAuth 2.1\n  evidence: The client discovers that https://inkseal.net/mcp is an OAuth protected resource and finds our authorization server.\n  how_to_obtain: The client discovers that https://inkseal.net/mcp is an OAuth protected resource and finds our authorization server.\ndocs: https://inkseal.net/docs/agents/oauth.md\n"
source_yaml_url: https://artifacts.apis.io/inkseal-net/authentication/inkseal-net-authentication.yml
summary_line: 2 schemes
tags:
- E-Signature
- Developer API
- Credit Pricing
---
