---
anonymous_access: false
api_key_in: []
api_specs:
- filename: barker-money-openapi-generated.yml
  format: yaml
  label: Barker Money API
  slug: barker-money-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/barker-money/openapi/_ae-authored/barker-money-openapi-generated.yml
auth_types: []
description: Barker Money uses a simple API key scheme.
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Barker Money Authentication
name_suffix: Authentication
oauth_flows: []
overview: Barker Money declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Barker Money
provider_slug: barker-money
scheme_count: 1
schemes:
- evidence: 'Every request must include:


    ```

    X-Api-Key: bk_live_xxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx

    ```'
  header: X-Api-Key
  how_to_obtain: Create a new key in Portal → API Keys (the key is returned once in plaintext).
  location: header
  name: API Key
  type: apiKey
slug: barker-money-authentication
source_filename: barker-money-authentication.yml
source_heading: Authentication Profile
source_url: https://docs.barker.money/authentication.md
source_yaml: "generated: '2026-11-02'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://docs.barker.money/authentication.md\nsources:\n- https://docs.barker.money/authentication.md\n- https://docs.barker.money/quickstart.md\ndescription: Barker Money uses a simple API key scheme.\nschemes:\n- type: apiKey\n  name: API Key\n  evidence: 'Every request must include:\n\n\n    ```\n\n    X-Api-Key: bk_live_xxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx\n\n    ```'\n  location: header\n  header: X-Api-Key\n  how_to_obtain: Create a new key in Portal → API Keys (the key is returned once in plaintext).\nnote: No OAuth2, HTTP‑basic, bearer, JWT, HMAC, or mTLS schemes are documented.\ndocs: https://docs.barker.money/authentication.md\n"
source_yaml_url: https://artifacts.apis.io/barker-money/authentication/barker-money-authentication.yml
summary_line: 1 scheme
tags:
- Finance
- Cryptocurrency
- Yield
- DeFi
- AgentEconomy
---
