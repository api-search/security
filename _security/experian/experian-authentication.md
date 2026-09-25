---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: experian-address-validation-api-openapi.yml
  format: yaml
  label: Experian Address Validation API
  slug: experian-address-validation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/experian/refs/heads/main/openapi/experian-address-validation-api-openapi.yml
- filename: experian-bulk-address-api-openapi.yml
  format: yaml
  label: Experian Bulk Address API
  slug: experian-bulk-address-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/experian/refs/heads/main/openapi/experian-bulk-address-api-openapi.yml
- filename: experian-bulk-email-api-openapi.yml
  format: yaml
  label: Experian Bulk Email API
  slug: experian-bulk-email-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/experian/refs/heads/main/openapi/experian-bulk-email-api-openapi.yml
- filename: experian-bulk-phone-api-openapi.yml
  format: yaml
  label: Experian Bulk Phone API
  slug: experian-bulk-phone-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/experian/refs/heads/main/openapi/experian-bulk-phone-api-openapi.yml
- filename: experian-email-validation-api-openapi.yml
  format: yaml
  label: Experian Email Validation API
  slug: experian-email-validation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/experian/refs/heads/main/openapi/experian-email-validation-api-openapi.yml
- filename: experian-enrichment-api-openapi.yml
  format: yaml
  label: Experian Enrichment API
  slug: experian-enrichment-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/experian/refs/heads/main/openapi/experian-enrichment-api-openapi.yml
- filename: experian-identity-append-usa-only-api-openapi.yml
  format: yaml
  label: Experian Identity Append (USA only) API
  slug: experian-identity-append-usa-only-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/experian/refs/heads/main/openapi/experian-identity-append-usa-only-api-openapi.yml
- filename: experian-phone-validation-api-openapi.yml
  format: yaml
  label: Experian Phone Validation API
  slug: experian-phone-validation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/experian/refs/heads/main/openapi/experian-phone-validation-api-openapi.yml
- filename: experian-reverse-phone-append-usa-only-api-openapi.yml
  format: yaml
  label: Experian Reverse Phone Append (USA only) API
  slug: experian-reverse-phone-append-usa-only-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/experian/refs/heads/main/openapi/experian-reverse-phone-append-usa-only-api-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
mechanism_count: 3
method: searched
name: Experian Authentication
name_suffix: Authentication
oauth_flows: []
overview: Experian secures its APIs with apiKey and http across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Experian
provider_slug: experian
scheme_count: 3
schemes:
- bearerFormat: JWT
  description: "Token URL: https://sso.experianaperture.io/oauth2/aust0wkxjeKyT3HRO4x7/v1/token \n\n Flow: clientCredentials"
  name: OAuth2
  scheme: Bearer
  sources:
  - openapi/experian-addressvalidation-openapi.json
  - openapi/experian-aperture-openapi.json
  - openapi/experian-bulkaddress-openapi.json
  - openapi/experian-bulkemail-openapi.json
  - openapi/experian-bulkphone-openapi.json
  - openapi/experian-emailvalidation-openapi.json
  - openapi/experian-emailvalidationv2-openapi.json
  - openapi/experian-enrichment-openapi.json
  - openapi/experian-identityappend-openapi.json
  - openapi/experian-phonevalidation-openapi.json
  - openapi/experian-reversephoneappend-openapi.json
  type: http
- description: Your unique key, called a token, that is required to submit an API request.
  in: header
  name: Auth-Token
  parameter: Auth-Token
  sources:
  - openapi/experian-addressvalidation-openapi.json
  - openapi/experian-aperture-openapi.json
  - openapi/experian-bulkaddress-openapi.json
  - openapi/experian-bulkemail-openapi.json
  - openapi/experian-bulkphone-openapi.json
  - openapi/experian-emailvalidation-openapi.json
  - openapi/experian-emailvalidationv2-openapi.json
  - openapi/experian-enrichment-openapi.json
  - openapi/experian-identityappend-openapi.json
  - openapi/experian-phonevalidation-openapi.json
  - openapi/experian-reversephoneappend-openapi.json
  type: apiKey
- description: Alternative Auth Token header.
  in: header
  name: x-app-key
  parameter: x-app-key
  sources:
  - openapi/experian-addressvalidation-openapi.json
  - openapi/experian-aperture-openapi.json
  - openapi/experian-bulkaddress-openapi.json
  - openapi/experian-bulkemail-openapi.json
  - openapi/experian-bulkphone-openapi.json
  - openapi/experian-emailvalidation-openapi.json
  - openapi/experian-emailvalidationv2-openapi.json
  - openapi/experian-enrichment-openapi.json
  - openapi/experian-identityappend-openapi.json
  - openapi/experian-phonevalidation-openapi.json
  - openapi/experian-reversephoneappend-openapi.json
  type: apiKey
slug: experian-authentication
source_filename: experian-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-13'\nmethod: searched\ndocs:\n- https://developer.experian.com/tutorials/oauth-20-tutorial\n- https://developer.experian.com/tutorials/quick-start-guide\n- https://docs.experianaperture.io/address-validation/experian-address-validation/get-started/securing-your-integration/\n- https://docs.experianaperture.io/more/self-service-portal/\nnote: 'Baseline derived from the eleven published OpenAPI documents, then upgraded from the two\n  provider documentation sets. Experian runs TWO different authentication models on two platforms and\n  the spec only describes one of them. Aperture (api.experianaperture.io): a static Auth-Token header\n  issued per integration from the Self Service Portal, with x-app-key documented as an alternative\n  header carrying the same value, plus an OAuth2 clientCredentials flow against the Okta issuer\n  sso.experianaperture.io. Entitlement is additionally bounded by per-integration domain and IP\n  allowlists — a valid token presented\
  \ from an unlisted domain or IP returns 403, which is a genuine\n  second factor most API providers do not offer. Global Developer Platform (developer.experian.com):\n  OAuth2 resource-owner password grant against the regional host''s own /oauth2/v1/token, using the\n  developer''s portal username and password together with an application client_id and\n  client_secret, returning a Bearer access token and a refresh token. Every region runs its own\n  issuer; ten of them serve a live OIDC discovery document (see well-known/). No product scopes exist\n  on either platform — see scopes/experian-scopes.yml.'\nplatforms:\n- platform: Experian Data Quality (Aperture)\n  primary: Auth-Token header\n  alternative_header: x-app-key\n  oauth2_flow: clientCredentials\n  token_endpoint: https://sso.experianaperture.io/oauth2/aust0wkxjeKyT3HRO4x7/v1/token\n  issuer: https://sso.experianaperture.io\n  issued_from: https://docs.experianaperture.io/more/self-service-portal/\n  additional_controls:\n \
  \ - per-integration domain allowlist\n  - per-integration IP allowlist\n  key_prefix_convention: none — environment is selected by hostname, not by key shape\n  rotation: managed in the Self Service Portal; no rotation API\n- platform: Experian Global Developer Platform\n  primary: OAuth2 resource-owner password grant\n  token_endpoint_pattern: https://{region-host}/oauth2/v1/token\n  credentials:\n  - Developer Portal username and password\n  - application client_id and client_secret from \"My Apps\"\n  returns:\n  - Bearer access_token\n  - refresh_token\n  issuers: see scopes/experian-scopes.yml — ten regional issuers, each serving OIDC discovery\n  deprecated_grant_note: The password grant is deprecated in OAuth 2.1 and the current OAuth security\n    BCP. Recorded as observed fact, not endorsed.\n  source: https://developer.experian.com/tutorials/quick-start-guide\nauth_failure_semantics:\n  '401': The Auth-Token provided is incorrect.\n  '403':\n  - token is valid but associated\
  \ with another product, or the account has insufficient credits\n  - token is disabled and must be activated in the Self Service Portal\n  - the calling domain is not on the integration allowlist\n  - the calling IP is not on the integration allowlist\n  source: errors/experian-problem-types.yml\nsource: openapi/experian-addressvalidation-openapi.json, openapi/experian-aperture-openapi.json,\n  openapi/experian-bulkaddress-openapi.json, openapi/experian-bulkemail-openapi.json, openapi/experian-bulkphone-openapi.json,\n  openapi/experian-emailvalidation-openapi.json, openapi/experian-emailvalidationv2-openapi.json,\n  openapi/experian-enrichment-openapi.json, openapi/experian-identityappend-openapi.json, openapi/experian-phonevalidation-openapi.json,\n  openapi/experian-reversephoneappend-openapi.json\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: OAuth2\n  type: http\n  scheme: Bearer\n  bearerFormat: JWT\n  description: \"Token URL: https://sso.experianaperture.io/oauth2/aust0wkxjeKyT3HRO4x7/v1/token\\\
  \n    \\ \\n\\n Flow: clientCredentials\"\n  sources:\n  - openapi/experian-addressvalidation-openapi.json\n  - openapi/experian-aperture-openapi.json\n  - openapi/experian-bulkaddress-openapi.json\n  - openapi/experian-bulkemail-openapi.json\n  - openapi/experian-bulkphone-openapi.json\n  - openapi/experian-emailvalidation-openapi.json\n  - openapi/experian-emailvalidationv2-openapi.json\n  - openapi/experian-enrichment-openapi.json\n  - openapi/experian-identityappend-openapi.json\n  - openapi/experian-phonevalidation-openapi.json\n  - openapi/experian-reversephoneappend-openapi.json\n- name: Auth-Token\n  type: apiKey\n  in: header\n  parameter: Auth-Token\n  description: Your unique key, called a token, that is required to submit an API request.\n  sources:\n  - openapi/experian-addressvalidation-openapi.json\n  - openapi/experian-aperture-openapi.json\n  - openapi/experian-bulkaddress-openapi.json\n  - openapi/experian-bulkemail-openapi.json\n  - openapi/experian-bulkphone-openapi.json\n\
  \  - openapi/experian-emailvalidation-openapi.json\n  - openapi/experian-emailvalidationv2-openapi.json\n  - openapi/experian-enrichment-openapi.json\n  - openapi/experian-identityappend-openapi.json\n  - openapi/experian-phonevalidation-openapi.json\n  - openapi/experian-reversephoneappend-openapi.json\n- name: x-app-key\n  type: apiKey\n  in: header\n  parameter: x-app-key\n  description: Alternative Auth Token header.\n  sources:\n  - openapi/experian-addressvalidation-openapi.json\n  - openapi/experian-aperture-openapi.json\n  - openapi/experian-bulkaddress-openapi.json\n  - openapi/experian-bulkemail-openapi.json\n  - openapi/experian-bulkphone-openapi.json\n  - openapi/experian-emailvalidation-openapi.json\n  - openapi/experian-emailvalidationv2-openapi.json\n  - openapi/experian-enrichment-openapi.json\n  - openapi/experian-identityappend-openapi.json\n  - openapi/experian-phonevalidation-openapi.json\n  - openapi/experian-reversephoneappend-openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/experian/refs/heads/main/authentication/experian-authentication.yml
summary_line: apiKey/http · 3 schemes
tags:
- Company
- Credit Bureau
- Credit Reporting
- Identity Verification
- Fraud Prevention
- Data Quality
- Address Validation
- Email Verification
- Phone Validation
- Data Enrichment
- Financial Services
- Risk Management
---
