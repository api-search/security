---
api_key_in: []
auth_types:
- http
description: ''
kind: authentication
layout: security
method: searched
name: Bitsight Authentication
name_suffix: Authentication
oauth_flows: []
overview: BitSight secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: BitSight
provider_slug: bitsight
scheme_count: 1
schemes:
- description: All API requests authenticate via HTTP Basic authentication. The Bitsight API token is supplied as the username with an empty password (a trailing colon with nothing after it in curl's -u parameter). All requests must be made over HTTPS; calls over plain HTTP fail. Tokens are generated per user under Settings -> Account -> User Preferences -> Generate New Token; company/service tokens can be created by admin and VRM admin roles.
  name: apiTokenBasic
  scheme: basic
  sources:
  - docs
  token_management: https://help.bitsighttech.com/hc/en-us/articles/115014888388-API-Token-Management
  token_types: https://help.bitsighttech.com/hc/en-us/articles/25748078243735-API-Token-Types
  type: http
slug: bitsight-authentication
source_filename: bitsight-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: https://help.bitsighttech.com/hc/en-us/articles/115014888388-API-Token-Management\ndocs: https://help.bitsighttech.com/hc/en-us/articles/115014888388-API-Token-Management\nsummary:\n  types: [http]\n  http_schemes: [basic]\n  api_key_in: []\n  oauth2_flows: []\n  transport: https-only\nschemes:\n- name: apiTokenBasic\n  type: http\n  scheme: basic\n  description: >-\n    All API requests authenticate via HTTP Basic authentication. The Bitsight API\n    token is supplied as the username with an empty password (a trailing colon with\n    nothing after it in curl's -u parameter). All requests must be made over HTTPS;\n    calls over plain HTTP fail. Tokens are generated per user under Settings ->\n    Account -> User Preferences -> Generate New Token; company/service tokens can be\n    created by admin and VRM admin roles.\n  token_management: https://help.bitsighttech.com/hc/en-us/articles/115014888388-API-Token-Management\n\
  \  token_types: https://help.bitsighttech.com/hc/en-us/articles/25748078243735-API-Token-Types\n  sources: [docs]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bitsight/refs/heads/main/authentication/bitsight-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Security
- Cyber Risk
- Security Ratings
- Third-Party Risk Management
- Attack Surface Management
- Threat Intelligence
- Vendor Risk
---
