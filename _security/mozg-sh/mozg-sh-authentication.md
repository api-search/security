---
anonymous_access: false
api_key_in: []
api_specs:
- filename: mozg-sh-openapi-generated.yml
  format: yaml
  label: Mozg API
  slug: mozg-sh-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mozg-sh/openapi/_ae-authored/mozg-sh-openapi-generated.yml
auth_types: []
description: Authentication for Mozg is performed via a Bearer token sent in the Authorization header.
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Mozg Authentication
name_suffix: Authentication
oauth_flows: []
overview: Mozg declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Mozg
provider_slug: mozg-sh
scheme_count: 1
schemes:
- evidence: 'auth Authorization: Bearer <token from https://mozg.sh/settings/tokens>'
  header: Authorization
  how_to_obtain: Obtain a token from https://mozg.sh/settings/tokens
  location: header
  name: Bearer Token
  type: http-bearer
slug: mozg-sh-authentication
source_filename: mozg-sh-authentication.yml
source_heading: Authentication Profile
source_url: https://mozg.sh/b/mozg/better-auth
source_yaml: "generated: '2026-11-18'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://mozg.sh/b/mozg/better-auth\nsources:\n- https://mozg.sh/b/mozg/better-auth\ndescription: Authentication for Mozg is performed via a Bearer token sent in the Authorization header.\nschemes:\n- type: http-bearer\n  name: Bearer Token\n  evidence: 'auth Authorization: Bearer <token from https://mozg.sh/settings/tokens>'\n  location: header\n  header: Authorization\n  how_to_obtain: Obtain a token from https://mozg.sh/settings/tokens\ndocs: https://mozg.sh/b/mozg/better-auth\n"
source_yaml_url: https://artifacts.apis.io/mozg-sh/authentication/mozg-sh-authentication.yml
summary_line: 1 scheme
tags:
- Company
- Artificial Intelligence
- Platform
- Open Source
- MCP
---
