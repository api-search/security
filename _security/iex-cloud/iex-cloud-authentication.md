---
api_key_in:
- query
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Iex Cloud Authentication
name_suffix: Authentication
oauth_flows: []
overview: IEX Cloud secures its APIs with apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: IEX Cloud
provider_slug: iex-cloud
scheme_count: 2
schemes:
- description: 'Publishable (public) API tokens granted Core dataset read access by default; could additionally be granted Premium Data access and per-dataset read/write/delete permissions. Supported optional restrictions: allowed domains, and core-credit usage limits per token.'
  in: query
  name: publishableToken
  parameter: token
  sources:
  - https://github.com/iexcloud/docs/blob/main/source/administration/access-and-security.md
  type: apiKey
- description: Secret tokens allowed any action on data and account; docs warned never to share them publicly. Hidden from dataset overview pages as of 2022-12-06.
  in: query
  name: secretToken
  parameter: token
  sources:
  - https://github.com/iexcloud/docs/blob/main/source/administration/access-and-security.md
  type: apiKey
slug: iex-cloud-authentication
source_filename: iex-cloud-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-22'\nmethod: searched\nsource: https://raw.githubusercontent.com/iexcloud/docs/main/source/administration/access-and-security.md\ndocs: https://github.com/iexcloud/docs/blob/main/source/administration/access-and-security.md\nnotes: >-\n  IEX Cloud sunset on 2024-08-31; this profile is preserved from the official\n  documentation source that survives in the public github.com/iexcloud/docs\n  repository (Apperate era). No live endpoints accept these credentials anymore.\nsummary:\n  types: [apiKey]\n  api_key_in: [query]\n  oauth2_flows: []\nschemes:\n  - name: publishableToken\n    type: apiKey\n    in: query\n    parameter: token\n    description: >-\n      Publishable (public) API tokens granted Core dataset read access by default;\n      could additionally be granted Premium Data access and per-dataset\n      read/write/delete permissions. Supported optional restrictions: allowed\n      domains, and core-credit usage limits per token.\n    sources:\n \
  \     - https://github.com/iexcloud/docs/blob/main/source/administration/access-and-security.md\n  - name: secretToken\n    type: apiKey\n    in: query\n    parameter: token\n    description: >-\n      Secret tokens allowed any action on data and account; docs warned never to\n      share them publicly. Hidden from dataset overview pages as of 2022-12-06.\n    sources:\n      - https://github.com/iexcloud/docs/blob/main/source/administration/access-and-security.md\nfeatures:\n  signed_requests: >-\n    Tokens could require a signature per request (available to Business plan and\n    legacy Grow/Scale users on legacy plans).\n  domain_restriction: >-\n    Tokens could be restricted to requests originating from specified domains.\n  per_token_limits: Core-credit usage limits could be set per token.\n  token_tiers: Launch up to 2 tokens, Grow up to 50, Scale up to 1,000 (Apperate limits page).\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/iex-cloud/refs/heads/main/authentication/iex-cloud-authentication.yml
summary_line: apiKey · 2 schemes
tags:
- Fintech
- Market Data
- Stocks
- Reference
- Sunset
- Historical
---
