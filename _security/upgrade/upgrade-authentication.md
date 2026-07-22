---
api_key_in: []
api_specs:
- filename: upgrade-flexpay-openapi.yml
  format: yaml
  label: Flex Pay API
  slug: flex-pay-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/upgrade/refs/heads/main/openapi/upgrade-flexpay-openapi.yml
auth_types:
- oauth2
description: Authentication profile for the Flex Pay APIs (Upgrade). Both the marketing and checkout REST APIs use OAuth 2.0 — an access token obtained with the client-credentials grant (client ID/secret sent as Basic credentials to the token endpoint) and included as a Bearer token in the Authorization header of every API request. Credentials are issued per merchant and per environment by the Flex Pay integration team, gated on a server IP allowlist review.
kind: authentication
layout: security
method: searched
name: Upgrade Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: Upgrade secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: Upgrade
provider_slug: upgrade
scheme_count: 1
schemes:
- flows:
  - flow: clientCredentials
    scopes: []
    tokenUrl: https://partner.upgrade.com/api/auth/v1/oauth/token?grant_type=client_credentials
    tokenUrl_preprod: https://partner.credify.tech/api/auth/v1/oauth/token?grant_type=client_credentials
    token_request_auth: 'Authorization: Basic {base64_encoded_credentials}'
  name: flexPayOAuth
  sources:
  - openapi/upgrade-flexpay-openapi.yml
  type: oauth2
slug: upgrade-authentication
source_filename: upgrade-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://docs.uplift.com/apidocs/authorization-1\ndocs: https://docs.uplift.com/apidocs/authorization-1\ndescription: >-\n  Authentication profile for the Flex Pay APIs (Upgrade). Both the marketing and\n  checkout REST APIs use OAuth 2.0 — an access token obtained with the\n  client-credentials grant (client ID/secret sent as Basic credentials to the\n  token endpoint) and included as a Bearer token in the Authorization header of\n  every API request. Credentials are issued per merchant and per environment by\n  the Flex Pay integration team, gated on a server IP allowlist review.\nsummary:\n  types: [oauth2]\n  oauth2_flows: [clientCredentials]\n  token_usage: 'Authorization: Bearer {token}'\n  token_expiry: 30 minutes (default) — refresh shortly before expiry\n  ip_allowlist_required: true\nschemes:\n  - name: flexPayOAuth\n    type: oauth2\n    flows:\n      - flow: clientCredentials\n        tokenUrl: https://partner.upgrade.com/api/auth/v1/oauth/token?grant_type=client_credentials\n\
  \        tokenUrl_preprod: https://partner.credify.tech/api/auth/v1/oauth/token?grant_type=client_credentials\n        token_request_auth: 'Authorization: Basic {base64_encoded_credentials}'\n        scopes: []\n    sources: [openapi/upgrade-flexpay-openapi.yml]\nendpoints:\n  production: https://partner.upgrade.com/api/flexpay\n  pre_production: https://partner.credify.tech/api/flexpay\ncredential_issuance: >-\n  Client IDs and client secrets are generated on a per-merchant and\n  per-environment basis during onboarding. A comprehensive list of server IP\n  addresses must be provided for security review before pre-production and\n  production credentials are issued.\nbest_practices:\n  - Share secrets only over secure channels (never email or unencrypted HTTP).\n  - Store secrets in a secrets manager, KMS, or encrypted database — never in code repositories or client-side code.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/upgrade/refs/heads/main/authentication/upgrade-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Company
- Fintech
- Lending
- Buy Now Pay Later
- Payments
- Credit Cards
- Banking
- Travel
---
