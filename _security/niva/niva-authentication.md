---
anonymous_access: false
api_key_in: []
api_specs:
- filename: niva-openapi-generated.yml
  format: yaml
  label: Niva API
  slug: niva-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/niva/openapi/_ae-authored/niva-openapi-generated.yml
auth_types: []
description: Token‑based authentication using an API token supplied in a custom header.
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Niva Authentication
name_suffix: Authentication
oauth_flows: []
overview: Niva declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Niva
provider_slug: niva
scheme_count: 1
schemes:
- evidence: To authenticate your API requests, include the `apiKey` header with the token in your HTTP request.
  header: apiKey
  how_to_obtain: Login to the Niva portal and generate a new API token; the token is then provided to you for use in requests.
  location: header
  name: apiKey
  type: apiKey
slug: niva-authentication
source_filename: niva-authentication.yml
source_heading: Authentication Profile
source_url: https://docs.niva.co/doc-598665.md
source_yaml: "generated: '2026-10-24'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://docs.niva.co/doc-598665.md\nsources:\n- https://docs.niva.co/doc-598665.md\n- https://docs.niva.co/doc-598721.md\ndescription: Token‑based authentication using an API token supplied in a custom header.\nschemes:\n- type: apiKey\n  name: apiKey\n  evidence: To authenticate your API requests, include the `apiKey` header with the token in your HTTP request.\n  location: header\n  header: apiKey\n  how_to_obtain: Login to the Niva portal and generate a new API token; the token is then provided to you for use in requests.\ndocs: https://docs.niva.co/doc-598665.md\n"
source_yaml_url: https://artifacts.apis.io/niva/authentication/niva-authentication.yml
summary_line: 1 scheme
tags:
- Company
- FinTech
- IdentityVerification
- AI
- Compliance
---
