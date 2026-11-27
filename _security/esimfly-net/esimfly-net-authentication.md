---
anonymous_access: false
api_key_in: []
api_specs:
- filename: esimfly-net-openapi-generated.yml
  format: yaml
  label: eSIMfly API
  slug: esimfly-net-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/esimfly-net/openapi/_ae-authored/esimfly-net-openapi-generated.yml
auth_types: []
description: The eSIMfly Business API uses HMAC‑SHA256 signature authentication.
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: eSIMfly Authentication
name_suffix: Authentication
oauth_flows: []
overview: eSIMfly declares 4 security scheme(s) across its OpenAPI definitions.
provider_name: eSIMfly
provider_slug: esimfly-net
scheme_count: 4
schemes:
- evidence: The eSIMfly Business API uses HMAC‑SHA256 signature authentication to ensure maximum security for all API requests.
  header: RT-AccessCode
  how_to_obtain: Log in to your eSIMfly Business Dashboard → Settings → API Keys → Create New API Key and save the access_code and secret_key.
  location: header
  name: HMAC Signature Authentication
  type: hmac
- evidence: The eSIMfly Business API uses HMAC‑SHA256 signature authentication to ensure maximum security for all API requests.
  header: RT-RequestID
  location: header
  name: HMAC Signature Authentication
  type: hmac
- evidence: The eSIMfly Business API uses HMAC‑SHA256 signature authentication to ensure maximum security for all API requests.
  header: RT-Timestamp
  location: header
  name: HMAC Signature Authentication
  type: hmac
- evidence: The eSIMfly Business API uses HMAC‑SHA256 signature authentication to ensure maximum security for all API requests.
  header: RT-Signature
  location: header
  name: HMAC Signature Authentication
  type: hmac
slug: esimfly-net-authentication
source_filename: esimfly-net-authentication.yml
source_heading: Authentication Profile
source_url: https://docs.esimfly.net/docs/api-authentication
source_yaml: "generated: '2026-11-07'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://docs.esimfly.net/docs/api-authentication\nsources:\n- https://docs.esimfly.net/docs/api-authentication\n- https://docs.esimfly.net/docs/quick-start\n- https://docs.esimfly.net/docs/intro\ndescription: The eSIMfly Business API uses HMAC‑SHA256 signature authentication.\nschemes:\n- type: hmac\n  name: HMAC Signature Authentication\n  evidence: The eSIMfly Business API uses HMAC‑SHA256 signature authentication to ensure maximum security for all API requests.\n  location: header\n  header: RT-AccessCode\n  how_to_obtain: Log in to your eSIMfly Business Dashboard → Settings → API Keys → Create New API Key and save the access_code and secret_key.\n- type: hmac\n  name: HMAC Signature Authentication\n  evidence: The eSIMfly Business API uses HMAC‑SHA256 signature authentication to ensure maximum security for all API requests.\n  location: header\n  header: RT-RequestID\n- type:\
  \ hmac\n  name: HMAC Signature Authentication\n  evidence: The eSIMfly Business API uses HMAC‑SHA256 signature authentication to ensure maximum security for all API requests.\n  location: header\n  header: RT-Timestamp\n- type: hmac\n  name: HMAC Signature Authentication\n  evidence: The eSIMfly Business API uses HMAC‑SHA256 signature authentication to ensure maximum security for all API requests.\n  location: header\n  header: RT-Signature\nnote: 'All required authentication information is sent via HTTP headers: RT-AccessCode, RT-RequestID, RT-Timestamp, and RT-Signature.'\ndocs: https://docs.esimfly.net/docs/api-authentication\n"
source_yaml_url: https://artifacts.apis.io/esimfly-net/authentication/esimfly-net-authentication.yml
summary_line: 4 schemes
tags:
- Company
- eSIM
- Travel
- Connectivity
- Telecommunications
---
