---
anonymous_access: false
api_key_in: []
api_specs:
- filename: wisepim-gtin-api-openapi.yml
  format: yaml
  label: WISEPIM Open Data API GTIN API
  slug: wisepim-gtin-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/wisepim/openapi/wisepim-gtin-api-openapi.yml
- filename: wisepim-hs-codes-api-openapi.yml
  format: yaml
  label: WISEPIM Open Data API HS codes API
  slug: wisepim-hs-codes-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/wisepim/openapi/wisepim-hs-codes-api-openapi.yml
- filename: wisepim-marketplace-fees-api-openapi.yml
  format: yaml
  label: WISEPIM Open Data API Marketplace fees API
  slug: wisepim-marketplace-fees-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/wisepim/openapi/wisepim-marketplace-fees-api-openapi.yml
auth_types: []
description: Authentication methods for WISEPIM
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: WISEPIM Open Data API Authentication
name_suffix: Authentication
oauth_flows: []
overview: WISEPIM Open Data API declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: WISEPIM Open Data API
provider_slug: wisepim
scheme_count: 2
schemes:
- evidence: 'Project API keys have no programmatic registration. A **project owner or admin** signs in to the WISEPIM app, opens **Settings > API Access**, clicks **Create API key**, names it and selects scopes:'
  header: Authorization
  how_to_obtain: A human creates the key in Settings > API Access in the WISEPIM app; the full `wpk_...` value is shown once after creation.
  location: header
  name: Project API key
  type: apiKey
- evidence: For Connected Apps, the assistant starts the OAuth request with `response_type=code`, a `code_challenge` (S256), the resource it wants to reach and the scopes it needs.
  how_to_obtain: The user initiates the OAuth consent flow via Connected Apps; the assistant exchanges the authorization code for an access token using PKCE.
  name: Connected Apps OAuth
  type: oauth2
slug: wisepim-authentication
source_filename: wisepim-authentication.yml
source_heading: Authentication Profile
source_url: https://docs.wisepim.com/auth.md
source_yaml: "generated: '2026-11-03'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://docs.wisepim.com/auth.md\nsources:\n- https://docs.wisepim.com/auth.md\n- https://wisepim.com/developers/api/authentication\n- https://wisepim.com/developers/api\ndescription: Authentication methods for WISEPIM\nschemes:\n- type: apiKey\n  name: Project API key\n  evidence: 'Project API keys have no programmatic registration. A **project owner or admin** signs in to the WISEPIM app, opens **Settings >\n    API Access**, clicks **Create API key**, names it and selects scopes:'\n  location: header\n  header: Authorization\n  how_to_obtain: A human creates the key in Settings > API Access in the WISEPIM app; the full `wpk_...` value is shown once after creation.\n- type: oauth2\n  name: Connected Apps OAuth\n  evidence: For Connected Apps, the assistant starts the OAuth request with `response_type=code`, a `code_challenge` (S256), the resource it wants\n    to reach and the\
  \ scopes it needs.\n  how_to_obtain: The user initiates the OAuth consent flow via Connected Apps; the assistant exchanges the authorization code for an access token\n    using PKCE.\ndocs: https://docs.wisepim.com/auth.md\n"
source_yaml_url: https://artifacts.apis.io/wisepim/authentication/wisepim-authentication.yml
summary_line: 2 schemes
tags:
- Product Information Management
- Artificial Intelligence
- E-Commerce
- Catalog Enrichment
- Translation
- Wholesale
- Retail
---
