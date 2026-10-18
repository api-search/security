---
anonymous_access: false
api_key_in: []
api_specs:
- filename: igrant-io-config-api-openapi.yml
  format: yaml
  label: iGrant.io Config API
  slug: igrant-io-config-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/igrant-io/refs/heads/main/openapi/igrant-io-config-api-openapi.yml
auth_types: []
description: Authentication
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Igrant Io Authentication
name_suffix: Authentication
oauth_flows: []
overview: iGrant.io declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: iGrant.io
provider_slug: igrant-io
scheme_count: 1
schemes:
- evidence: 'Send the key as `Authorization: ApiKey <apiKey>`.'
  header: Authorization
  how_to_obtain: Send an email to iGrant.io Developer Support to obtain your API keys.
  location: header
  name: ApiKey
  type: apiKey
slug: igrant-io-authentication
source_filename: igrant-io-authentication.yml
source_heading: Authentication Profile
source_url: https://docs.igrant.io/docs/developer-apis/get-started/
source_yaml: "generated: '2026-10-15'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://docs.igrant.io/docs/developer-apis/get-started/\nsources:\n- https://docs.igrant.io/docs/developer-apis/get-started/\n- https://docs.igrant.io/docs/category/openid4vc-api/key-management/\n- https://docs.igrant.io/docs/category/openid4vc-api/api-key/\n- https://docs.igrant.io/docs/openid4vc-api/config-list-digital-wallet-open-id-scopes/\ndescription: Authentication\nschemes:\n- type: apiKey\n  name: ApiKey\n  evidence: 'Send the key as `Authorization: ApiKey <apiKey>`.'\n  location: header\n  header: Authorization\n  how_to_obtain: Send an email to iGrant.io Developer Support to obtain your API keys.\nnote: No OAuth2 or other authentication schemes are documented on the provided pages.\ndocs: https://docs.igrant.io/docs/developer-apis/get-started/\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/igrant-io/refs/heads/main/authentication/igrant-io-authentication.yml
summary_line: 1 scheme
tags:
- Company
- Identity
- Wallets
- eIDAS
---
