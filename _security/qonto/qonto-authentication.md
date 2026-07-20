---
api_key_in: []
api_specs:
- filename: qonto-openapi.yml
  format: yaml
  label: Qonto Business API
  slug: qonto-business-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/qonto/refs/heads/main/openapi/qonto-openapi.yml
- filename: qonto-openapi.yml
  format: yaml
  label: Qonto Transactions & Statements API
  slug: qonto-transactions-statements-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/qonto/refs/heads/main/openapi/qonto-openapi.yml
- filename: qonto-openapi.yml
  format: yaml
  label: Qonto SEPA Transfers API
  slug: qonto-sepa-transfers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/qonto/refs/heads/main/openapi/qonto-openapi.yml
- filename: qonto-openapi.yml
  format: yaml
  label: Qonto International Transfers API
  slug: qonto-international-transfers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/qonto/refs/heads/main/openapi/qonto-openapi.yml
- filename: qonto-openapi.yml
  format: yaml
  label: Qonto Internal Transfers API
  slug: qonto-internal-transfers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/qonto/refs/heads/main/openapi/qonto-openapi.yml
- filename: qonto-openapi.yml
  format: yaml
  label: Qonto Cards API
  slug: qonto-cards-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/qonto/refs/heads/main/openapi/qonto-openapi.yml
- filename: qonto-openapi.yml
  format: yaml
  label: Qonto Client Invoices & Quotes API
  slug: qonto-client-invoices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/qonto/refs/heads/main/openapi/qonto-openapi.yml
- filename: qonto-openapi.yml
  format: yaml
  label: Qonto Supplier Invoices API
  slug: qonto-supplier-invoices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/qonto/refs/heads/main/openapi/qonto-openapi.yml
- filename: qonto-openapi.yml
  format: yaml
  label: Qonto SEPA Direct Debit API
  slug: qonto-sepa-direct-debit-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/qonto/refs/heads/main/openapi/qonto-openapi.yml
- filename: qonto-openapi.yml
  format: yaml
  label: Qonto Payment Links API
  slug: qonto-payment-links-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/qonto/refs/heads/main/openapi/qonto-openapi.yml
- filename: qonto-openapi.yml
  format: yaml
  label: Qonto Terminals API
  slug: qonto-terminals-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/qonto/refs/heads/main/openapi/qonto-openapi.yml
- filename: qonto-openapi.yml
  format: yaml
  label: Qonto Webhooks API
  slug: qonto-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/qonto/refs/heads/main/openapi/qonto-openapi.yml
- filename: qonto-openapi.yml
  format: yaml
  label: Qonto Onboarding API
  slug: qonto-onboarding-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/qonto/refs/heads/main/openapi/qonto-openapi.yml
- filename: qonto-openapi.yml
  format: yaml
  label: Qonto Embed SDK & Hosted Pages API
  slug: qonto-embed-sdk-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/qonto/refs/heads/main/openapi/qonto-openapi.yml
auth_types:
- apiKey
- oauth2
- mtls
description: ''
kind: authentication
layout: security
method: documented
name: Qonto Authentication
name_suffix: Authentication
oauth_flows: []
overview: Qonto secures its APIs with apiKey, oauth2, and mtls across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Qonto
provider_slug: qonto
scheme_count: 3
schemes:
- format: '{sign-in}:{secret-key}'
  headerName: Authorization
  in: header
  name: secret_key
  note: Organization sign-in and secret key concatenated with a colon in the Authorization header. Resembles HTTP Basic authentication but is NOT - the value is not Base64 encoded. Generated from the Qonto app under Integrations and Partnerships > API key.
  sources:
  - https://docs.qonto.com/get-started/business-api/authentication/api-key
  type: apiKey
- accessTokenTtlSeconds: 3600
  flow: authorizationCode
  name: oauth2
  note: OAuth 2.0 authorization code flow; recommended for SaaS integrations. Access token valid 1 hour, refresh token 90 days (offline_access scope), ID token via openid scope. Client secret must only be used server-side. Per-resource scopes (e.g. organization.read, payment.write, card.write, sepa_direct_debit.write, webhook). A User OAuth flow enables access across multiple organizations of the same user.
  refreshTokenTtlDays: 90
  sources:
  - https://docs.qonto.com/api-reference/business-api/authentication/oauth2/create_tokens
  - https://docs.qonto.com/get-started/business-api/authentication/oauth/oauth-flow
  - https://docs.qonto.com/get-started/business-api/authentication/oauth/available-scopes
  supportsOpenIdConnect: true
  tokenUrl: https://thirdparty.qonto.com/oauth2/token
  type: oauth2
- name: qsealc
  note: Regulated Third-Party Providers (TPPs) identify themselves via a PSD2 QSeal certificate for open-banking access.
  sources:
  - https://docs.qonto.com/get-started/business-api/authentication/qsealc
  standard: PSD2 QSeal certificate (QSealC)
  type: mtls
slug: qonto-authentication
source_filename: qonto-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: documented\nsource: https://docs.qonto.com/get-started/business-api/authentication/api-key\nsummary:\n  types:\n  - apiKey\n  - oauth2\n  - mtls\nschemes:\n- name: secret_key\n  type: apiKey\n  in: header\n  headerName: Authorization\n  format: '{sign-in}:{secret-key}'\n  note: >-\n    Organization sign-in and secret key concatenated with a colon in the\n    Authorization header. Resembles HTTP Basic authentication but is NOT - the\n    value is not Base64 encoded. Generated from the Qonto app under Integrations\n    and Partnerships > API key.\n  sources:\n  - https://docs.qonto.com/get-started/business-api/authentication/api-key\n- name: oauth2\n  type: oauth2\n  flow: authorizationCode\n  tokenUrl: https://thirdparty.qonto.com/oauth2/token\n  accessTokenTtlSeconds: 3600\n  refreshTokenTtlDays: 90\n  supportsOpenIdConnect: true\n  note: >-\n    OAuth 2.0 authorization code flow; recommended for SaaS integrations. Access\n    token valid 1\
  \ hour, refresh token 90 days (offline_access scope), ID token via\n    openid scope. Client secret must only be used server-side. Per-resource scopes\n    (e.g. organization.read, payment.write, card.write, sepa_direct_debit.write,\n    webhook). A User OAuth flow enables access across multiple organizations of the\n    same user.\n  sources:\n  - https://docs.qonto.com/api-reference/business-api/authentication/oauth2/create_tokens\n  - https://docs.qonto.com/get-started/business-api/authentication/oauth/oauth-flow\n  - https://docs.qonto.com/get-started/business-api/authentication/oauth/available-scopes\n- name: qsealc\n  type: mtls\n  standard: PSD2 QSeal certificate (QSealC)\n  note: >-\n    Regulated Third-Party Providers (TPPs) identify themselves via a PSD2 QSeal\n    certificate for open-banking access.\n  sources:\n  - https://docs.qonto.com/get-started/business-api/authentication/qsealc\nadditionalControls:\n- name: Strong Customer Authentication (SCA)\n  applies_to:\n  - SEPA\
  \ transfers\n  - bulk transfers\n  - international transfers\n  headers:\n  - X-Qonto-Sca-Session-Token\n  - X-Qonto-MFA\n  - X-Qonto-2fa-Preference\n  note: >-\n    PSD2 Strong Customer Authentication is enforced on sensitive money-movement\n    operations; the client drives an SCA session and supplies the session token /\n    MFA challenge headers. Trusted beneficiaries (Embed partners only) can bypass\n    per-transfer SCA.\n  sources:\n  - https://docs.qonto.com/api-reference/business-api/authentication/sca/sca-flows\n- name: Idempotency\n  headers:\n  - X-Qonto-Idempotency-Key\n  note: Client-generated key to safely retry create requests without duplication.\n  sources:\n  - https://docs.qonto.com/get-started/general/idempotent-requests\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/qonto/refs/heads/main/authentication/qonto-authentication.yml
summary_line: apiKey/oauth2/mtls · 3 schemes
tags:
- Business Banking
- Neobank
- Fintech
- Payments
- SEPA
- Open Banking
- EUR
- Europe
---
