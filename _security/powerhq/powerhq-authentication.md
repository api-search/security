---
anonymous_access: false
api_key_in: []
auth_types: []
description: PowerHQ uses a single API key authentication scheme.
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Powerhq Authentication
name_suffix: Authentication
oauth_flows: []
overview: PowerHQ declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: PowerHQ
provider_slug: powerhq
scheme_count: 1
schemes:
- evidence: 'Authenticate every PowerHQ API request with your API key: one static secret in the x-api-key header, no OAuth handshake, no token to refresh.'
  header: x-api-key
  how_to_obtain: Contact your partner manager to receive your key.
  location: header
  name: API Key
  type: apiKey
slug: powerhq-authentication
source_filename: powerhq-authentication.yml
source_heading: Authentication Profile
source_url: https://docs.powerhq.co/authentication.md
source_yaml: "generated: '2026-10-02'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://docs.powerhq.co/authentication.md\nsources:\n- https://docs.powerhq.co/authentication.md\n- https://docs.powerhq.co/quickstart.md\ndescription: PowerHQ uses a single API key authentication scheme.\nschemes:\n- type: apiKey\n  name: API Key\n  evidence: 'Authenticate every PowerHQ API request with your API key: one static secret in the x-api-key header, no OAuth handshake, no token\n    to refresh.'\n  location: header\n  header: x-api-key\n  how_to_obtain: Contact your partner manager to receive your key.\ndocs: https://docs.powerhq.co/authentication.md\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/powerhq/refs/heads/main/authentication/powerhq-authentication.yml
summary_line: 1 scheme
tags:
- Energy Commerce
- Retail Electricity
- Marketplace
- API
- Energy Providers
- Developers
- Partners
- Brokers
---
