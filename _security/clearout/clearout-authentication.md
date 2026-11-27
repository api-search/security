---
anonymous_access: false
api_key_in: []
api_specs:
- filename: clearout-openapi-generated.yml
  format: yaml
  label: Clearout API
  slug: clearout-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/clearout/openapi/_ae-authored/clearout-openapi-generated.yml
auth_types: []
description: Authentication methods as published by Clearout
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Clearout Authentication
name_suffix: Authentication
oauth_flows: []
overview: Clearout declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Clearout
provider_slug: clearout
scheme_count: 1
schemes:
- authorize_url: https://app.clearout.io/oauth/authorize
  evidence: Clearout supports the OAuth 2.1 authorization-code flow with PKCE (`S256` only).
  how_to_obtain: Register an OAuth app in the Clearout Developer Console to obtain a Client ID (and Client Secret for confidential apps).
  name: Clearout OAuth 2.1
  scopes:
  - all_products
  - account
  type: oauth2
slug: clearout-authentication
source_filename: clearout-authentication.yml
source_heading: Authentication Profile
source_url: https://docs.clearout.io/developers/oauth-server.md
source_yaml: "generated: '2026-11-16'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://docs.clearout.io/developers/oauth-server.md\nsources:\n- https://docs.clearout.io/developers/oauth-server.md\n- https://docs.clearout.io/data-pulse/implementation-and-setup.md\ndescription: Authentication methods as published by Clearout\nschemes:\n- type: oauth2\n  name: Clearout OAuth 2.1\n  evidence: Clearout supports the OAuth 2.1 authorization-code flow with PKCE (`S256` only).\n  authorize_url: https://app.clearout.io/oauth/authorize\n  scopes:\n  - all_products\n  - account\n  how_to_obtain: Register an OAuth app in the Clearout Developer Console to obtain a Client ID (and Client Secret for confidential apps).\ndocs: https://docs.clearout.io/developers/oauth-server.md\n"
source_yaml_url: https://artifacts.apis.io/clearout/authentication/clearout-authentication.yml
summary_line: 1 scheme
tags:
- Company
- Email Verification
- Email Finder
- Sales Prospecting
- Data Enrichment
---
