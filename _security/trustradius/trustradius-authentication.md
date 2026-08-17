---
api_key_in:
- header
api_specs:
- filename: trustradius-product-data-api-openapi.yml
  format: yaml
  label: TrustRadius Product Data API
  slug: trustradius-product-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/trustradius/refs/heads/main/openapi/trustradius-product-data-api-openapi.yml
- filename: trustradius-intent-data-api-openapi.yml
  format: yaml
  label: TrustRadius Downstream Intent Data API
  slug: trustradius-intent-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/trustradius/refs/heads/main/openapi/trustradius-intent-data-api-openapi.yml
- filename: trustradius-trustquotes-api-openapi.yml
  format: yaml
  label: TrustRadius TrustQuotes Content Syndication API
  slug: trustradius-trustquotes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/trustradius/refs/heads/main/openapi/trustradius-trustquotes-api-openapi.yml
- filename: trustradius-traffic-data-api-openapi.yml
  format: yaml
  label: TrustRadius Traffic Data API
  slug: trustradius-traffic-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/trustradius/refs/heads/main/openapi/trustradius-traffic-data-api-openapi.yml
- filename: trustradius-legacy-api-openapi.yml
  format: yaml
  label: TrustRadius Legacy Visitor Insights API
  slug: trustradius-legacy-visitor-insights-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/trustradius/refs/heads/main/openapi/trustradius-legacy-api-openapi.yml
auth_types:
- apiKey
description: 'One authentication model: a single opaque API key, sent in the lowercase `x-api-key` HTTP header, issued per vendor account. There is no OAuth surface, no OIDC discovery, no scope model, no token exchange, no refresh, and no documented rotation or expiry policy. The key is the whole security contract.'
kind: authentication
layout: security
method: searched
name: Trustradius Authentication
name_suffix: Authentication
oauth_flows: []
overview: TrustRadius secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: TrustRadius
provider_slug: trustradius
scheme_count: 1
schemes:
- applied_to: all 11 published operations
  case_sensitive: true
  declared_at: operation level only
  declared_at_note: 'The published spec repeats `security: [{x-api-key: []}]` on each operation and declares no root-level `security` block, so a generator that reads only the document root will treat the API as unauthenticated.'
  description: All API calls must send an API key in the "x-api-key" HTTP header. TrustRadius clients can get their key from their Client Success Manager.
  in: header
  name: x-api-key
  parameter: x-api-key
  sources:
  - openapi/_original/trustradius-api-openapi.yml
  - openapi/trustradius-intent-data-api-openapi.yml
  - openapi/trustradius-legacy-api-openapi.yml
  - openapi/trustradius-product-data-api-openapi.yml
  - openapi/trustradius-traffic-data-api-openapi.yml
  - openapi/trustradius-trustquotes-api-openapi.yml
  type: apiKey
slug: trustradius-authentication
source_filename: trustradius-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-14'\nmethod: searched\nsource: >-\n  https://apidocs.trustradius.com/docs/public-api/ZG9jOjQ1Mg-trust-radius-api (auth section),\n  https://trustradius.freshdesk.com/support/solutions/articles/43000639047 (key retrieval),\n  openapi/_original/trustradius-api-openapi.yml (securitySchemes)\ndocs: https://apidocs.trustradius.com/docs/public-api/ZG9jOjQ1Mg-trust-radius-api\nprovider: TrustRadius\nproviderId: trustradius\ndescription: >-\n  One authentication model: a single opaque API key, sent in the lowercase `x-api-key` HTTP header,\n  issued per vendor account. There is no OAuth surface, no OIDC discovery, no scope model, no token\n  exchange, no refresh, and no documented rotation or expiry policy. The key is the whole security\n  contract.\nsummary:\n  types:\n    - apiKey\n  api_key_in:\n    - header\n  oauth2: false\n  oidc: false\n  mtls: false\n  scopes: false\nschemes:\n  - name: x-api-key\n    type: apiKey\n    in: header\n    parameter: x-api-key\n\
  \    case_sensitive: true\n    description: >-\n      All API calls must send an API key in the \"x-api-key\" HTTP header. TrustRadius clients can get\n      their key from their Client Success Manager.\n    applied_to: all 11 published operations\n    declared_at: operation level only\n    declared_at_note: >-\n      The published spec repeats `security: [{x-api-key: []}]` on each operation and declares no\n      root-level `security` block, so a generator that reads only the document root will treat the\n      API as unauthenticated.\n    sources:\n      - openapi/_original/trustradius-api-openapi.yml\n      - openapi/trustradius-intent-data-api-openapi.yml\n      - openapi/trustradius-legacy-api-openapi.yml\n      - openapi/trustradius-product-data-api-openapi.yml\n      - openapi/trustradius-traffic-data-api-openapi.yml\n      - openapi/trustradius-trustquotes-api-openapi.yml\ncredential_issuance:\n  self_serve: false\n  paths:\n    - name: Vendor Portal\n      steps: Log in to the\
  \ TrustRadius Vendor Portal > Integrations > \"Get API key\" > copy to clipboard.\n      url: https://trustradius.freshdesk.com/support/solutions/articles/43000639047\n    - name: Client Success Manager\n      steps: Ask your assigned TrustRadius CSM, or email product@trustradius.com.\n      url: https://apidocs.trustradius.com/docs/public-api/ZG9jOjQ1Mg-trust-radius-api\n  prerequisite: >-\n    A paid vendor subscription. There is no free tier, trial key, or developer signup — see plans/.\n  entitlement_note: >-\n    A valid key does not imply access to every endpoint. Which paths return data depends on the\n    package elements the vendor account holds (content licensing, visitor insights, category intent\n    data). A key without the relevant entitlement is denied with the same 403 as an invalid key.\ntransport:\n  https_only: true\n  quote: All API access is over HTTPS at https://api.trustradius.com/v1\n  example: \"curl -H 'x-api-key:VENDOR_AUTH_KEY' https://api.trustradius.com/v1\"\
  \nfailure_modes:\n  - status: 403\n    body: '{\"message\":\"Forbidden\"}'\n    causes:\n      - Missing x-api-key header.\n      - Invalid or revoked key.\n      - Vendor account not entitled to the requested path.\n    note: >-\n      The same status and body cover all three causes, so a client cannot tell a credential problem\n      from an entitlement problem from the response.\ngaps:\n  - No key rotation, expiry, or revocation policy is published.\n  - No scope or least-privilege model — one key grants everything the account is entitled to.\n  - No 401 is declared or observed; the edge answers 403 for unauthenticated requests.\n  - No /.well-known/oauth-authorization-server or /.well-known/openid-configuration on any host.\nmaintainers:\n  - FN: Kin Lane\n    email: kin@apievangelist.com\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/trustradius/refs/heads/main/authentication/trustradius-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- B2B Software Reviews
- Buyer Intelligence
- Intent Data
- Software Reviews
- Reviews
- Product Reviews
- Content Syndication
- Account Based Marketing
- Marketing
- Analytics
---
