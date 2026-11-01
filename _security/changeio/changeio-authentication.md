---
anonymous_access: false
api_key_in: []
auth_types: []
description: The Change API is authenticated using public and secret keys via HTTP Basic Auth.
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Changeio Authentication
name_suffix: Authentication
oauth_flows: []
overview: Change.io declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Change.io
provider_slug: changeio
scheme_count: 1
schemes:
- evidence: Authentication is perfomed with HTTP Basic Auth .
  header: Authorization
  how_to_obtain: Sign up for a Change account to get your public (pk_*) and secret (sk_*) keys.
  location: header
  name: Basic
  type: http-basic
slug: changeio-authentication
source_filename: changeio-authentication.yml
source_heading: Authentication Profile
source_url: https://docs.getchange.io/api/authentication/
source_yaml: "generated: '2026-10-26'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://docs.getchange.io/api/authentication/\nsources:\n- https://docs.getchange.io/api/authentication/\n- https://docs.getchange.io/api/authentication/\n- https://docs.getchange.io/getting-started/\ndescription: The Change API is authenticated using public and secret keys via HTTP Basic Auth.\nschemes:\n- type: http-basic\n  name: Basic\n  evidence: Authentication is perfomed with HTTP Basic Auth .\n  location: header\n  header: Authorization\n  how_to_obtain: Sign up for a Change account to get your public (pk_*) and secret (sk_*) keys.\nnote: No OAuth2, API key, bearer token, or other authentication schemes are documented.\ndocs: https://docs.getchange.io/api/authentication/\n"
source_yaml_url: https://artifacts.apis.io/changeio/authentication/changeio-authentication.yml
summary_line: 1 scheme
tags:
- Donations
- Compliance
- API
- Nonprofit Verification
- Disbursements
- Corporate Giving
- Legal Teams
- Charitable Registrations
---
