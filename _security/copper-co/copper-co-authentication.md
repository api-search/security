---
api_key_in:
- header
api_specs:
- filename: copper-co-accounts-api-openapi.yml
  format: yaml
  label: Copper.co Accounts API
  slug: copper-co-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/copper-co/refs/heads/main/openapi/copper-co-accounts-api-openapi.yml
- filename: copper-co-address-book-api-openapi.yml
  format: yaml
  label: Copper.co Address Book API
  slug: copper-co-address-book-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/copper-co/refs/heads/main/openapi/copper-co-address-book-api-openapi.yml
- filename: copper-co-blockchain-api-openapi.yml
  format: yaml
  label: Copper.co Blockchain API
  slug: copper-co-blockchain-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/copper-co/refs/heads/main/openapi/copper-co-blockchain-api-openapi.yml
- filename: copper-co-clearloop-api-openapi.yml
  format: yaml
  label: Copper.co Clearloop API
  slug: copper-co-clearloop-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/copper-co/refs/heads/main/openapi/copper-co-clearloop-api-openapi.yml
- filename: copper-co-currencies-api-openapi.yml
  format: yaml
  label: Copper.co Currencies API
  slug: copper-co-currencies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/copper-co/refs/heads/main/openapi/copper-co-currencies-api-openapi.yml
- filename: copper-co-deposit-targets-api-openapi.yml
  format: yaml
  label: Copper.co Deposit Targets API
  slug: copper-co-deposit-targets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/copper-co/refs/heads/main/openapi/copper-co-deposit-targets-api-openapi.yml
- filename: copper-co-exchange-api-openapi.yml
  format: yaml
  label: Copper.co Exchange API
  slug: copper-co-exchange-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/copper-co/refs/heads/main/openapi/copper-co-exchange-api-openapi.yml
- filename: copper-co-files-api-openapi.yml
  format: yaml
  label: Copper.co Files API
  slug: copper-co-files-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/copper-co/refs/heads/main/openapi/copper-co-files-api-openapi.yml
- filename: copper-co-lending-api-openapi.yml
  format: yaml
  label: Copper.co Lending API
  slug: copper-co-lending-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/copper-co/refs/heads/main/openapi/copper-co-lending-api-openapi.yml
- filename: copper-co-network-api-openapi.yml
  format: yaml
  label: Copper.co Network API
  slug: copper-co-network-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/copper-co/refs/heads/main/openapi/copper-co-network-api-openapi.yml
- filename: copper-co-orders-api-openapi.yml
  format: yaml
  label: Copper.co Orders API
  slug: copper-co-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/copper-co/refs/heads/main/openapi/copper-co-orders-api-openapi.yml
- filename: copper-co-organizations-api-openapi.yml
  format: yaml
  label: Copper.co Organizations API
  slug: copper-co-organizations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/copper-co/refs/heads/main/openapi/copper-co-organizations-api-openapi.yml
- filename: copper-co-portfolios-api-openapi.yml
  format: yaml
  label: Copper.co Portfolios API
  slug: copper-co-portfolios-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/copper-co/refs/heads/main/openapi/copper-co-portfolios-api-openapi.yml
- filename: copper-co-reports-api-openapi.yml
  format: yaml
  label: Copper.co Reports API
  slug: copper-co-reports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/copper-co/refs/heads/main/openapi/copper-co-reports-api-openapi.yml
- filename: copper-co-sign-async-api-openapi.yml
  format: yaml
  label: Copper.co Sign Async API
  slug: copper-co-sign-async-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/copper-co/refs/heads/main/openapi/copper-co-sign-async-api-openapi.yml
- filename: copper-co-stake-api-openapi.yml
  format: yaml
  label: Copper.co Stake API
  slug: copper-co-stake-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/copper-co/refs/heads/main/openapi/copper-co-stake-api-openapi.yml
- filename: copper-co-trades-api-openapi.yml
  format: yaml
  label: Copper.co Trades API
  slug: copper-co-trades-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/copper-co/refs/heads/main/openapi/copper-co-trades-api-openapi.yml
- filename: copper-co-wallets-api-openapi.yml
  format: yaml
  label: Copper.co Wallets API
  slug: copper-co-wallets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/copper-co/refs/heads/main/openapi/copper-co-wallets-api-openapi.yml
auth_types:
- apiKey
- httpSignature
description: ''
kind: authentication
layout: security
method: searched
name: Copper Co Authentication
name_suffix: Authentication
oauth_flows: []
overview: Copper.co secures its APIs with apiKey and httpSignature across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Copper.co
provider_slug: copper-co
scheme_count: 2
schemes:
- description: API key issued in the Copper Platform UI under Settings > API Keys. Keys may be owned by a user account or, recommended for integrations, by a service account so the key survives team changes. Keys can be restricted to an IP allowlist.
  in: header
  name: ApiKeyAuth
  parameter_name: Authorization
  sources:
  - https://developer.copper.co/api-reference/authentication
  - https://developer.copper.co/api-reference/create-api-key
  type: apiKey
  value_format: ApiKey {API_KEY}
- algorithm: HMAC-SHA256
  description: Per-request integrity signature. Every request must additionally carry X-Signature and X-Timestamp.
  encoding: hex
  in: header
  name: RequestSignature
  parameter_name: X-Signature
  sources:
  - https://developer.copper.co/api-reference/authentication
  type: httpSignature
slug: copper-co-authentication
source_filename: copper-co-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-04'\nmethod: searched\nsource: https://developer.copper.co/api-reference/authentication\ndocs: https://developer.copper.co/api-reference/authentication\nnote: >-\n  The published OpenAPI documents declare NO components.securitySchemes and apply no\n  security[] requirement, so the mechanical derive pass (derive-authentication.py)\n  returned an empty profile. This profile is therefore captured from the provider's\n  documentation, which describes the scheme in full. Documenting the scheme in the\n  spec is the single highest-value contract fix available to Copper.\nsummary:\n  types:\n  - apiKey\n  - httpSignature\n  api_key_in:\n  - header\n  oauth2_flows: []\n  signed_requests: true\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter_name: Authorization\n  value_format: ApiKey {API_KEY}\n  description: >-\n    API key issued in the Copper Platform UI under Settings > API Keys. Keys may be\n    owned by a user account or, recommended\
  \ for integrations, by a service account so\n    the key survives team changes. Keys can be restricted to an IP allowlist.\n  sources:\n  - https://developer.copper.co/api-reference/authentication\n  - https://developer.copper.co/api-reference/create-api-key\n- name: RequestSignature\n  type: httpSignature\n  in: header\n  parameter_name: X-Signature\n  algorithm: HMAC-SHA256\n  encoding: hex\n  description: >-\n    Per-request integrity signature. Every request must additionally carry X-Signature\n    and X-Timestamp.\n  sources:\n  - https://developer.copper.co/api-reference/authentication\nrequired_headers:\n- header: Authorization\n  description: API key obtained on the Copper Platform, in the form \"ApiKey {API_KEY}\".\n- header: X-Signature\n  description: Hex-encoded HMAC-SHA256 signature of the request.\n- header: X-Timestamp\n  description: Request timestamp as a UNIX timestamp in milliseconds.\n- header: Content-Type\n  description: application/json\nsignature:\n  algorithm:\
  \ HMAC-SHA256\n  encoding: hex\n  secret: API Secret issued alongside the API key\n  string_to_sign: '{X-Timestamp}{HTTP_METHOD_UPPERCASE}{path_including_/platform_prefix_and_query}{request_body}'\n  notes:\n  - Timestamp is milliseconds since the Unix epoch, not seconds.\n  - HTTP method must be uppercase.\n  - Path must include the /platform prefix and all query parameters, e.g. /platform/orders?limit=1000.\n  - Use an empty string for the body when the request has no body.\n  code_examples:\n  - bash\n  - python\n  - java\n  - go\n  - scala\nservice_accounts:\n  docs: https://developer.copper.co/api-reference/service-accounts\n  description: >-\n    Recommended owner for integration API keys. Permissions are granted per service\n    account and per portfolio.\n  permission_types:\n  - Trader\n  - Withdrawal Operator\n  - Loan Manager\n  - Approver\nip_allowlist:\n  supported: true\n  description: An API key may be restricted to a set of source IP addresses.\noauth2: false\nscopes_artifact:\
  \ null\nscopes_note: >-\n  Copper uses API-key + HMAC signature authentication with role-based service-account\n  permissions. There is no OAuth 2.0 surface and therefore no scope reference, so no\n  scopes/ artifact is emitted.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/copper-co/refs/heads/main/authentication/copper-co-authentication.yml
summary_line: apiKey/httpSignature · 2 schemes
tags:
- Company
- Digital Asset Custody
- Cryptocurrency
- Financial Services
- Institutional Finance
- Prime Brokerage
- Collateral Management
- Lending
- Settlement
- Staking
- Blockchain
- Treasury Management
---
