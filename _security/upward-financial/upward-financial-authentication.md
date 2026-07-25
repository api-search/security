---
api_key_in: []
api_specs:
- filename: upward-financial-accounts-api-openapi.yml
  format: yaml
  label: Upward Financial accounts API
  slug: upward-financial-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/upward-financial/refs/heads/main/openapi/upward-financial-accounts-api-openapi.yml
- filename: upward-financial-auth-api-openapi.yml
  format: yaml
  label: Upward Financial auth API
  slug: upward-financial-auth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/upward-financial/refs/heads/main/openapi/upward-financial-auth-api-openapi.yml
- filename: upward-financial-billpayments-api-openapi.yml
  format: yaml
  label: Upward Financial billPayments API
  slug: upward-financial-billpayments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/upward-financial/refs/heads/main/openapi/upward-financial-billpayments-api-openapi.yml
- filename: upward-financial-billreporting-api-openapi.yml
  format: yaml
  label: Upward Financial billReporting API
  slug: upward-financial-billreporting-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/upward-financial/refs/heads/main/openapi/upward-financial-billreporting-api-openapi.yml
- filename: upward-financial-billswitch-api-openapi.yml
  format: yaml
  label: Upward Financial billSwitch API
  slug: upward-financial-billswitch-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/upward-financial/refs/heads/main/openapi/upward-financial-billswitch-api-openapi.yml
- filename: upward-financial-cbaas-api-openapi.yml
  format: yaml
  label: Upward Financial cbaas API
  slug: upward-financial-cbaas-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/upward-financial/refs/heads/main/openapi/upward-financial-cbaas-api-openapi.yml
- filename: upward-financial-consumers-api-openapi.yml
  format: yaml
  label: Upward Financial consumers API
  slug: upward-financial-consumers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/upward-financial/refs/heads/main/openapi/upward-financial-consumers-api-openapi.yml
- filename: upward-financial-creditinsights-api-openapi.yml
  format: yaml
  label: Upward Financial creditInsights API
  slug: upward-financial-creditinsights-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/upward-financial/refs/heads/main/openapi/upward-financial-creditinsights-api-openapi.yml
- filename: upward-financial-onboarding-api-openapi.yml
  format: yaml
  label: Upward Financial onboarding API
  slug: upward-financial-onboarding-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/upward-financial/refs/heads/main/openapi/upward-financial-onboarding-api-openapi.yml
- filename: upward-financial-partners-api-openapi.yml
  format: yaml
  label: Upward Financial partners API
  slug: upward-financial-partners-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/upward-financial/refs/heads/main/openapi/upward-financial-partners-api-openapi.yml
- filename: upward-financial-paymentcards-api-openapi.yml
  format: yaml
  label: Upward Financial paymentCards API
  slug: upward-financial-paymentcards-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/upward-financial/refs/heads/main/openapi/upward-financial-paymentcards-api-openapi.yml
- filename: upward-financial-payments-api-openapi.yml
  format: yaml
  label: Upward Financial payments API
  slug: upward-financial-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/upward-financial/refs/heads/main/openapi/upward-financial-payments-api-openapi.yml
- filename: upward-financial-plaid-api-openapi.yml
  format: yaml
  label: Upward Financial plaid API
  slug: upward-financial-plaid-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/upward-financial/refs/heads/main/openapi/upward-financial-plaid-api-openapi.yml
- filename: upward-financial-rewards-api-openapi.yml
  format: yaml
  label: Upward Financial rewards API
  slug: upward-financial-rewards-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/upward-financial/refs/heads/main/openapi/upward-financial-rewards-api-openapi.yml
- filename: upward-financial-simulations-api-openapi.yml
  format: yaml
  label: Upward Financial simulations API
  slug: upward-financial-simulations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/upward-financial/refs/heads/main/openapi/upward-financial-simulations-api-openapi.yml
- filename: upward-financial-statements-api-openapi.yml
  format: yaml
  label: Upward Financial statements API
  slug: upward-financial-statements-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/upward-financial/refs/heads/main/openapi/upward-financial-statements-api-openapi.yml
- filename: upward-financial-webhooks-api-openapi.yml
  format: yaml
  label: Upward Financial webhooks API
  slug: upward-financial-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/upward-financial/refs/heads/main/openapi/upward-financial-webhooks-api-openapi.yml
auth_types:
- http
- oauth2
description: The Upward (Upwardli) Credit Suite API uses OAuth 2.0 for machine-to-machine authentication. Partners obtain a Bearer access token from the dedicated Authorization service (client_credentials grant with client_id + client_secret and requested scopes), then pass it in the Authorization header of every API request. A second endpoint implements RFC 8693 OAuth token exchange to down-scope a partner token to a single consumer (consumer:<upward_consumer_id>), producing a limited token that is safe to ship to a client application or browser. The OpenAPI declares the resulting Bearer scheme (http bearer).
kind: authentication
layout: security
method: searched
name: Upward Financial Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
- token-exchange (RFC 8693)
overview: Upward Financial secures its APIs with http and oauth2 across 3 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials and token-exchange (RFC 8693) flow(s).
provider_name: Upward Financial
provider_slug: upward-financial
scheme_count: 3
schemes:
- name: bearerAuth
  scheme: bearer
  sources:
  - openapi/upward-financial-openapi.json
  type: http
- flow: clientCredentials
  name: oauth2ClientCredentials
  notes: Documented on the developer portal (not declared in the OpenAPI, which only models the resulting Bearer header). Request body is JSON with grant_type, client_id, client_secret, and space-separated scope.
  sources:
  - https://developers.upwardli.com/concepts/authentication/o-auth-2-0
  tokenUrl: https://auth.upwardli.com/auth/token/
  type: oauth2
- flow: token-exchange
  grant_type: urn:ietf:params:oauth:grant-type:token-exchange
  name: oauth2TokenExchange
  notes: RFC 8693 token exchange. Exchanges a partner access_token for a consumer-scoped token (scope consumer:<upward_consumer_id>) with a 1-hour lifetime, safe to send to the client application.
  sources:
  - https://developers.upwardli.com/concepts/authentication/token-exchange
  tokenUrl: https://auth.upwardli.com/auth/token/exchange/
  type: oauth2
slug: upward-financial-authentication
source_filename: upward-financial-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: openapi/upward-financial-openapi.json\ndocs: https://developers.upwardli.com/concepts/authentication/introduction\ndescription: >-\n  The Upward (Upwardli) Credit Suite API uses OAuth 2.0 for machine-to-machine\n  authentication. Partners obtain a Bearer access token from the dedicated\n  Authorization service (client_credentials grant with client_id +\n  client_secret and requested scopes), then pass it in the Authorization\n  header of every API request. A second endpoint implements RFC 8693 OAuth\n  token exchange to down-scope a partner token to a single consumer\n  (consumer:<upward_consumer_id>), producing a limited token that is safe to\n  ship to a client application or browser. The OpenAPI declares the resulting\n  Bearer scheme (http bearer).\nsummary:\n  types:\n  - http\n  - oauth2\n  oauth2_flows:\n  - clientCredentials\n  - token-exchange (RFC 8693)\ntoken_endpoints:\n  sandbox: https://auth-sandbox.upwardli.com/auth/token/\n\
  \  production: https://auth.upwardli.com/auth/token/\ntoken_exchange_endpoints:\n  sandbox: https://auth-sandbox.upwardli.com/auth/token/exchange/\n  production: https://auth.upwardli.com/auth/token/exchange/\ntoken_lifetimes:\n  partner_access_token_seconds: 86400\n  exchanged_consumer_token_seconds: 3600\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  sources:\n  - openapi/upward-financial-openapi.json\n- name: oauth2ClientCredentials\n  type: oauth2\n  flow: clientCredentials\n  tokenUrl: https://auth.upwardli.com/auth/token/\n  notes: >-\n    Documented on the developer portal (not declared in the OpenAPI, which\n    only models the resulting Bearer header). Request body is JSON with\n    grant_type, client_id, client_secret, and space-separated scope.\n  sources:\n  - https://developers.upwardli.com/concepts/authentication/o-auth-2-0\n- name: oauth2TokenExchange\n  type: oauth2\n  flow: token-exchange\n  grant_type: urn:ietf:params:oauth:grant-type:token-exchange\n\
  \  tokenUrl: https://auth.upwardli.com/auth/token/exchange/\n  notes: >-\n    RFC 8693 token exchange. Exchanges a partner access_token for a\n    consumer-scoped token (scope consumer:<upward_consumer_id>) with a\n    1-hour lifetime, safe to send to the client application.\n  sources:\n  - https://developers.upwardli.com/concepts/authentication/token-exchange\nrelated:\n  scopes: scopes/upward-financial-scopes.yml\n  conventions: conventions/upward-financial-conventions.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/upward-financial/refs/heads/main/authentication/upward-financial-authentication.yml
summary_line: http/oauth2 · 3 schemes
tags:
- Company
- FinTech
- Credit
- Credit Building
- Payments
- Cards
- Embedded Finance
- Bill Pay
- Banking
- KYC
---
