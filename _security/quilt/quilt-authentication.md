---
anonymous_access: false
api_key_in: []
api_specs:
- filename: quilt-openapi-generated.yml
  format: yaml
  label: Quilt API
  slug: quilt-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/quilt/openapi/_ae-authored/quilt-openapi-generated.yml
auth_types: []
description: Authentication methods described in Quilt documentation
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Quilt Authentication
name_suffix: Authentication
oauth_flows: []
overview: Quilt declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Quilt
provider_slug: quilt
scheme_count: 2
schemes:
- evidence: Interactive authentication uses OAuth or SSO to authenticate through your web browser.
  how_to_obtain: Run `quilt3.login()` which opens a browser for OAuth/SSO authentication.
  name: Interactive Login
  type: oauth2
- evidence: API keys provide programmatic access to Quilt without requiring browser-based authentication.
  how_to_obtain: Create an API key via `quilt3.api_keys.create(...)` after an interactive login, then use `quilt3.login_with_api_key(api_key, registry_url=...)`.
  name: API Key
  type: apiKey
slug: quilt-authentication
source_filename: quilt-authentication.yml
source_heading: Authentication Profile
source_url: https://docs.quilt.bio/quilt-python-sdk/api-reference/authentication.md
source_yaml: "generated: '2026-10-24'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://docs.quilt.bio/quilt-python-sdk/api-reference/authentication.md\nsources:\n- https://docs.quilt.bio/quilt-python-sdk/api-reference/authentication.md\n- https://docs.quilt.bio/quilt-python-sdk/quickstart.md\ndescription: Authentication methods described in Quilt documentation\nschemes:\n- type: oauth2\n  name: Interactive Login\n  evidence: Interactive authentication uses OAuth or SSO to authenticate through your web browser.\n  how_to_obtain: Run `quilt3.login()` which opens a browser for OAuth/SSO authentication.\n- type: apiKey\n  name: API Key\n  evidence: API keys provide programmatic access to Quilt without requiring browser-based authentication.\n  how_to_obtain: Create an API key via `quilt3.api_keys.create(...)` after an interactive login, then use `quilt3.login_with_api_key(api_key,\n    registry_url=...)`.\ndocs: https://docs.quilt.bio/quilt-python-sdk/api-reference/authentication.md\n"
source_yaml_url: https://artifacts.apis.io/quilt/authentication/quilt-authentication.yml
summary_line: 2 schemes
tags:
- Company
- Data Platform
- Life Sciences
- AI
---
