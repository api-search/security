---
anonymous_access: false
api_key_in: []
api_specs:
- filename: lighthorse-io-cash-api-openapi.yml
  format: yaml
  label: Light Horse Cash API
  slug: lighthorse-io-cash-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lighthorse-io/openapi/lighthorse-io-cash-api-openapi.yml
auth_types: []
description: Authentication schemes for Light Horse API
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Light Horse Authentication
name_suffix: Authentication
oauth_flows: []
overview: Light Horse declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Light Horse
provider_slug: lighthorse-io
scheme_count: 2
schemes:
- evidence: Every request to the Light Horse API must include both an API key and a cryptographic signature.
  header: x-trade-apikey
  how_to_obtain: A unique ID issued when your API key pair is created.
  location: header
  name: x-trade-apikey
  type: apiKey
- evidence: Every request to the Light Horse API must include both an API key and a cryptographic signature.
  header: x-trade-signature
  how_to_obtain: Computed by HMAC‑SHA256 over the request data using your API secret and then Base64‑encoded.
  location: header
  name: x-trade-signature
  type: other
slug: lighthorse-io-authentication
source_filename: lighthorse-io-authentication.yml
source_heading: Authentication Profile
source_url: https://www.lighthorse.io/docs/authentication
source_yaml: "generated: '2026-11-15'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://www.lighthorse.io/docs/authentication\nsources:\n- https://www.lighthorse.io/docs/authentication\n- https://www.lighthorse.io/docs/authentication.md\n- https://www.lighthorse.io/instructions/getting-started/changelog\n- https://www.lighthorse.io/instructions/getting-started/download-mobile\ndescription: Authentication schemes for Light Horse API\nschemes:\n- type: apiKey\n  name: x-trade-apikey\n  evidence: Every request to the Light Horse API must include both an API key and a cryptographic signature.\n  location: header\n  header: x-trade-apikey\n  how_to_obtain: A unique ID issued when your API key pair is created.\n- type: other\n  name: x-trade-signature\n  evidence: Every request to the Light Horse API must include both an API key and a cryptographic signature.\n  location: header\n  header: x-trade-signature\n  how_to_obtain: Computed by HMAC‑SHA256 over the request\
  \ data using your API secret and then Base64‑encoded.\ndocs: https://www.lighthorse.io/docs/authentication\n"
source_yaml_url: https://artifacts.apis.io/lighthorse-io/authentication/lighthorse-io-authentication.yml
summary_line: 2 schemes
tags:
- Company
- Artificial Intelligence
- Brokerage
- Finance
- Trading
---
