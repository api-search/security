---
anonymous_access: false
api_key_in: []
auth_types: []
description: Authentication schemes for Chkk API
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Chkk Authentication
name_suffix: Authentication
oauth_flows: []
overview: Chkk declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Chkk
provider_slug: chkk
scheme_count: 1
schemes:
- evidence: 'description: Authorization credentials supplied in the Authorization header.'
  header: Authorization
  how_to_obtain: Create a token in the Chkk Dashboard under Settings → Tokens, then copy the token and use it in the Authorization header.
  location: header
  name: bearer_token
  type: apiKey
slug: chkk-authentication
source_filename: chkk-authentication.yml
source_heading: Authentication Profile
source_url: https://docs.chkk.io/administration/access-tokens.md
source_yaml: "generated: '2026-10-23'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://docs.chkk.io/administration/access-tokens.md\nsources:\n- https://docs.chkk.io/administration/access-tokens.md\n- https://docs.chkk.io/api-reference/v1/login/get-access-token.md\n- https://docs.chkk.io/overview/quickstart-chkk-cli.md\n- https://docs.chkk.io/overview/quickstart-chkk-dashboard.md\ndescription: Authentication schemes for Chkk API\nschemes:\n- type: apiKey\n  name: bearer_token\n  evidence: 'description: Authorization credentials supplied in the Authorization header.'\n  location: header\n  header: Authorization\n  how_to_obtain: Create a token in the Chkk Dashboard under Settings → Tokens, then copy the token and use it in the Authorization header.\nnote: No OAuth2, http-bearer, http-basic, jwt, hmac, mtls, or other schemes are documented.\ndocs: https://docs.chkk.io/administration/access-tokens.md\n"
source_yaml_url: https://artifacts.apis.io/chkk/authentication/chkk-authentication.yml
summary_line: 1 scheme
tags:
- Lifecycle Management
- Kubernetes
- Cloud Native
- Enterprise Software
---
