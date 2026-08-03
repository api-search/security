---
api_key_in:
- header
api_specs:
- filename: bolt-financial-bolt-api-openapi.yml
  format: yaml
  label: Bolt API
  slug: bolt-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bolt-financial/refs/heads/main/openapi/bolt-financial-bolt-api-openapi.yml
- filename: bolt-financial-embeddable-checkout-v1-openapi.yml
  format: yaml
  label: Bolt Embeddable Checkout v1 API
  slug: embeddable-checkout-v1
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bolt-financial/refs/heads/main/openapi/bolt-financial-embeddable-checkout-v1-openapi.yml
- filename: bolt-financial-embeddable-checkout-v3-openapi.yml
  format: yaml
  label: Bolt Embeddable Checkout v3 API
  slug: embeddable-checkout-v3
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bolt-financial/refs/heads/main/openapi/bolt-financial-embeddable-checkout-v3-openapi.yml
- filename: bolt-financial-tokenizer-openapi.yml
  format: yaml
  label: Bolt Tokenizer API
  slug: tokenizer
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bolt-financial/refs/heads/main/openapi/bolt-financial-tokenizer-openapi.yml
auth_types:
- apiKey
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Bolt Financial Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Bolt Financial secures its APIs with apiKey and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Bolt Financial
provider_slug: bolt-financial
scheme_count: 2
schemes:
- description: 'Bolt utilizes the OAuth flow that developers can use to attain access to Bolt Account data via APIs.

    For all APIs that require authorization, please provide your `access_token` returned from `/v1/oauth/token` via the basic auth bearer header `Authorization: bearer ${TOKEN}`.

    [Read more about the OAuth token endpoint.](/api-bolt/#tag/OAuth)'
  flows:
  - authorizationUrl: https://api.boltapp.com/v1/oauth/authorize
    flow: authorizationCode
    scopes: 3
    tokenUrl: https://api.boltapp.com/v1/oauth/token
  name: OAuth
  sources:
  - openapi/bolt-financial-bolt-api-openapi.yml
  - openapi/bolt-financial-embeddable-checkout-v1-openapi.yml
  - openapi/bolt-financial-embeddable-checkout-v3-openapi.yml
  type: oauth2
- description: Admins and Developers can obtain their Bolt API key from the Bolt Merchant Dashboard.
  in: header
  name: X-API-Key
  parameter: X-API-Key
  sources:
  - openapi/bolt-financial-bolt-api-openapi.yml
  - openapi/bolt-financial-embeddable-checkout-v1-openapi.yml
  - openapi/bolt-financial-embeddable-checkout-v3-openapi.yml
  type: apiKey
slug: bolt-financial-authentication
source_filename: bolt-financial-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-31'\nmethod: searched\ndocs: https://help.boltapp.com/developers/tools/api-keys/\noauth_docs: https://help.boltapp.com/developers/bolt-oauth/\nsource: openapi/bolt-financial-bolt-api-openapi.yml, openapi/bolt-financial-embeddable-checkout-v1-openapi.yml,\n  openapi/bolt-financial-embeddable-checkout-v3-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - oauth2\n  api_key_in:\n  - header\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: OAuth\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://api.boltapp.com/v1/oauth/authorize\n    tokenUrl: https://api.boltapp.com/v1/oauth/token\n    scopes: 3\n  description: |-\n    Bolt utilizes the OAuth flow that developers can use to attain access to Bolt Account data via APIs.\n    For all APIs that require authorization, please provide your `access_token` returned from `/v1/oauth/token` via the basic auth bearer header `Authorization: bearer ${TOKEN}`.\n    [Read more about\
  \ the OAuth token endpoint.](/api-bolt/#tag/OAuth)\n  sources:\n  - openapi/bolt-financial-bolt-api-openapi.yml\n  - openapi/bolt-financial-embeddable-checkout-v1-openapi.yml\n  - openapi/bolt-financial-embeddable-checkout-v3-openapi.yml\n- name: X-API-Key\n  type: apiKey\n  in: header\n  parameter: X-API-Key\n  description: Admins and Developers can obtain their Bolt API key from the Bolt Merchant Dashboard.\n  sources:\n  - openapi/bolt-financial-bolt-api-openapi.yml\n  - openapi/bolt-financial-embeddable-checkout-v1-openapi.yml\n  - openapi/bolt-financial-embeddable-checkout-v3-openapi.yml\ncredentials:\n- name: API Key\n  header: X-Api-Key\n  purpose: Server-side calls from the merchant backend to the Bolt API.\n  notes: Up to five active API keys per merchant; rotatable with no downtime from the Merchant\n    Dashboard (Administration > API).\n  source: https://help.boltapp.com/developers/tools/api-keys/\n- name: Signing Secret\n  header: X-Bolt-Hmac-Sha256\n  rotation_header: X-Bolt-Hmac-Sha256-Pending\n\
  \  purpose: HMAC-SHA256 signature verification of inbound Bolt webhooks and Merchant Callback\n    requests.\n  notes: Rotation supports an Active + Pending pair; reverting to the previous secret is possible\n    for up to 48 hours.\n  source: https://help.boltapp.com/developers/tools/api-keys/\n- name: Publishable Key\n  purpose: Client-side SDK initialization; also serves as the OAuth client_id.\n  source: https://help.boltapp.com/developers/bolt-oauth/\nrequired_headers:\n- header: X-Api-Key\n  value: the merchant API key\n- header: X-Nonce\n  value: unique 12-16 digit value per request (UUID recommended)\n- header: Content-Type\n  value: application/json\noauth:\n  grant: authorization_code\n  client_id: merchant publishable key\n  client_secret: merchant API key\n  authorization_code_ttl: 5 minutes\n  access_token_ttl: 1 hour\n  refresh_token_ttl: 1 year (single use)\n  refresh_token_rotation: true\n  token_presentation: 'Authorization: Bearer ${TOKEN}'\n  oidc: true\n  oidc_discovery:\
  \ https://api.boltapp.com/.well-known/openid-configuration\n  id_token_alg: RS256\n  jwks_uri: https://api.boltapp.com/v1/oauth/jwks.json\n  docs: https://help.boltapp.com/developers/bolt-oauth/\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bolt-financial/refs/heads/main/authentication/bolt-financial-authentication.yml
summary_line: apiKey/oauth2 · 2 schemes
tags:
- Company
- Payments
- Checkout
- eCommerce
- Fintech
- Subscriptions
- Tokenization
- Fraud
- Identity
- Webhooks
---
