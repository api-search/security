---
anonymous_access: false
api_key_in: []
api_specs:
- filename: cryptodecentral-co-za-content-api-openapi.yml
  format: yaml
  label: CryptoDecentral Content API
  slug: cryptodecentral-co-za-content-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cryptodecentral-co-za/openapi/cryptodecentral-co-za-content-api-openapi.yml
- filename: cryptodecentral-co-za-directory-api-openapi.yml
  format: yaml
  label: CryptoDecentral Directory API
  slug: cryptodecentral-co-za-directory-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cryptodecentral-co-za/openapi/cryptodecentral-co-za-directory-api-openapi.yml
- filename: cryptodecentral-co-za-discovery-api-openapi.yml
  format: yaml
  label: CryptoDecentral Discovery API
  slug: cryptodecentral-co-za-discovery-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cryptodecentral-co-za/openapi/cryptodecentral-co-za-discovery-api-openapi.yml
- filename: cryptodecentral-co-za-meta-api-openapi.yml
  format: yaml
  label: CryptoDecentral Meta API
  slug: cryptodecentral-co-za-meta-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cryptodecentral-co-za/openapi/cryptodecentral-co-za-meta-api-openapi.yml
auth_types: []
description: Authentication schemes published by CryptoDecentral
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Cryptodecentral Co Za Authentication
name_suffix: Authentication
oauth_flows: []
overview: CryptoDecentral declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: CryptoDecentral
provider_slug: cryptodecentral-co-za
scheme_count: 1
schemes:
- evidence: NIP-42 (draft, optional, relay-facing) adds a bidirectional AUTH frame on the WebSocket.
  how_to_obtain: Client signs an ephemeral event of kind 22242 containing the relay URL and challenge string and sends it as a WebSocket AUTH message.
  location: body
  name: NIP-42 AUTH
  type: other
slug: cryptodecentral-co-za-authentication
source_filename: cryptodecentral-co-za-authentication.yml
source_heading: Authentication Profile
source_url: https://cryptodecentral.co.za/notes/nostrbook-mcp-read-only-signing-line
source_yaml: "generated: '2026-11-04'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://cryptodecentral.co.za/notes/nostrbook-mcp-read-only-signing-line\nsources:\n- https://cryptodecentral.co.za/notes/nostrbook-mcp-read-only-signing-line\n- https://cryptodecentral.co.za/notes/nostr-nip42-auth-challenge-response\n- https://cryptodecentral.co.za/notes/self-custody-psbt-airgapped-signing\ndescription: Authentication schemes published by CryptoDecentral\nschemes:\n- type: other\n  name: NIP-42 AUTH\n  evidence: NIP-42 (draft, optional, relay-facing) adds a bidirectional AUTH frame on the WebSocket.\n  location: body\n  how_to_obtain: Client signs an ephemeral event of kind 22242 containing the relay URL and challenge string and sends it as a WebSocket AUTH\n    message.\ndocs: https://cryptodecentral.co.za/notes/nostrbook-mcp-read-only-signing-line\n"
source_yaml_url: https://artifacts.apis.io/cryptodecentral-co-za/authentication/cryptodecentral-co-za-authentication.yml
summary_line: 1 scheme
tags:
- Cryptocurrency
- Decentralization
- Privacy
- Education
- Sovereign Internet
---
