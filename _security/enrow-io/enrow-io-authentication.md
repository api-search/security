---
anonymous_access: false
api_key_in: []
api_specs:
- filename: enrow-io-openapi-generated.yml
  format: yaml
  label: Enrow API
  slug: enrow-io-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/enrow-io/openapi/_ae-authored/enrow-io-openapi-generated.yml
auth_types: []
description: Enrow API uses a single API key authentication scheme.
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Enrow Authentication
name_suffix: Authentication
oauth_flows: []
overview: Enrow declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Enrow
provider_slug: enrow-io
scheme_count: 1
schemes:
- evidence: The Enrow API uses API key authentication. Every request must include your API key in the `x-api-key` header.
  header: x-api-key
  how_to_obtain: Sign up at https://app.enrow.io, click **API** in the left menu, and copy your API key.
  location: header
  name: API Key
  type: apiKey
slug: enrow-io-authentication
source_filename: enrow-io-authentication.yml
source_heading: Authentication Profile
source_url: https://docs.enrow.io/authentication.md
source_yaml: "generated: '2026-11-06'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://docs.enrow.io/authentication.md\nsources:\n- https://docs.enrow.io/authentication.md\n- https://docs.enrow.io/da/playbooks/make/getting-started.md\n- https://docs.enrow.io/da/playbooks/n8n/getting-started.md\n- https://docs.enrow.io/da/playbooks/zapier/getting-started.md\ndescription: Enrow API uses a single API key authentication scheme.\nschemes:\n- type: apiKey\n  name: API Key\n  evidence: The Enrow API uses API key authentication. Every request must include your API key in the `x-api-key` header.\n  location: header\n  header: x-api-key\n  how_to_obtain: Sign up at https://app.enrow.io, click **API** in the left menu, and copy your API key.\nnote: There are no OAuth2 flows, bearer tokens, or other authentication methods documented.\ndocs: https://docs.enrow.io/authentication.md\n"
source_yaml_url: https://artifacts.apis.io/enrow-io/authentication/enrow-io-authentication.yml
summary_line: 1 scheme
tags:
- B2B
- Contact Data
- Sales Enablement
- Email Finder
- Phone Finder
---
