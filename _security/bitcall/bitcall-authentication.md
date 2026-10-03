---
anonymous_access: false
api_key_in: []
auth_types: []
description: Authenticate requests to the gateway with your key id and secret.
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Bitcall Authentication
name_suffix: Authentication
oauth_flows: []
overview: Bitcall declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Bitcall
provider_slug: bitcall
scheme_count: 2
schemes:
- evidence: 'Every request to a /v1/* endpoint is authenticated with two headers: your key id and your secret , both sent as-is.'
  header: x-key-id
  how_to_obtain: Create a key from your panel; the key id and secret are shown once at creation.
  location: header
  name: API Key
  type: apiKey
- evidence: 'Every request to a /v1/* endpoint is authenticated with two headers: your key id and your secret , both sent as-is.'
  header: x-api-secret
  how_to_obtain: Create a key from your panel; the secret is shown once at creation.
  location: header
  name: API Secret
  type: apiKey
slug: bitcall-authentication
source_filename: bitcall-authentication.yml
source_heading: Authentication Profile
source_url: https://docs.bitcall.io/docs/authentication
source_yaml: "generated: '2026-10-03'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://docs.bitcall.io/docs/authentication\nsources:\n- https://docs.bitcall.io/docs/authentication\n- https://docs.bitcall.io/docs/gateway/managing-api-keys\n- https://docs.bitcall.io/docs/gateway/api-keys\n- https://docs.bitcall.io/docs/quickstart\ndescription: Authenticate requests to the gateway with your key id and secret.\nschemes:\n- type: apiKey\n  name: API Key\n  evidence: 'Every request to a /v1/* endpoint is authenticated with two headers: your key id and your secret , both sent as-is.'\n  location: header\n  header: x-key-id\n  how_to_obtain: Create a key from your panel; the key id and secret are shown once at creation.\n- type: apiKey\n  name: API Secret\n  evidence: 'Every request to a /v1/* endpoint is authenticated with two headers: your key id and your secret , both sent as-is.'\n  location: header\n  header: x-api-secret\n  how_to_obtain: Create a key from your\
  \ panel; the secret is shown once at creation.\nnote: Both headers must be sent on every request.\ndocs: https://docs.bitcall.io/docs/authentication\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bitcall/refs/heads/main/authentication/bitcall-authentication.yml
summary_line: 2 schemes
tags:
- Telecom
- VoIP
- SMS
- eSIM
- API
---
