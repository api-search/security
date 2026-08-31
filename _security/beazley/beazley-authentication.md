---
api_key_in:
- header
- query
api_specs:
- filename: beazley-audit-api-openapi.yml
  format: yaml
  label: Beazley Audit API
  slug: beazley-audit-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/beazley/refs/heads/main/openapi/beazley-audit-api-openapi.yml
- filename: beazley-check-api-openapi.yml
  format: yaml
  label: Beazley Check API
  slug: beazley-check-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/beazley/refs/heads/main/openapi/beazley-check-api-openapi.yml
- filename: beazley-contacts-api-openapi.yml
  format: yaml
  label: Beazley Contacts API
  slug: beazley-contacts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/beazley/refs/heads/main/openapi/beazley-contacts-api-openapi.yml
- filename: beazley-currencies-api-openapi.yml
  format: yaml
  label: Beazley Currencies API
  slug: beazley-currencies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/beazley/refs/heads/main/openapi/beazley-currencies-api-openapi.yml
- filename: beazley-cyber-api-openapi.yml
  format: yaml
  label: Beazley Cyber API
  slug: beazley-cyber-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/beazley/refs/heads/main/openapi/beazley-cyber-api-openapi.yml
- filename: beazley-definitions-api-openapi.yml
  format: yaml
  label: Beazley Definitions API
  slug: beazley-definitions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/beazley/refs/heads/main/openapi/beazley-definitions-api-openapi.yml
- filename: beazley-faqs-api-openapi.yml
  format: yaml
  label: Beazley Faqs API
  slug: beazley-faqs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/beazley/refs/heads/main/openapi/beazley-faqs-api-openapi.yml
- filename: beazley-health-api-openapi.yml
  format: yaml
  label: Beazley Health API
  slug: beazley-health-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/beazley/refs/heads/main/openapi/beazley-health-api-openapi.yml
- filename: beazley-lockstate-api-openapi.yml
  format: yaml
  label: Beazley Lockstate API
  slug: beazley-lockstate-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/beazley/refs/heads/main/openapi/beazley-lockstate-api-openapi.yml
- filename: beazley-microsites-api-openapi.yml
  format: yaml
  label: Beazley Microsites API
  slug: beazley-microsites-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/beazley/refs/heads/main/openapi/beazley-microsites-api-openapi.yml
- filename: beazley-organisations-api-openapi.yml
  format: yaml
  label: Beazley Organisations API
  slug: beazley-organisations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/beazley/refs/heads/main/openapi/beazley-organisations-api-openapi.yml
- filename: beazley-people-api-openapi.yml
  format: yaml
  label: Beazley People API
  slug: beazley-people-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/beazley/refs/heads/main/openapi/beazley-people-api-openapi.yml
- filename: beazley-ping-api-openapi.yml
  format: yaml
  label: Beazley Ping API
  slug: beazley-ping-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/beazley/refs/heads/main/openapi/beazley-ping-api-openapi.yml
- filename: beazley-products-api-openapi.yml
  format: yaml
  label: Beazley Products API
  slug: beazley-products-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/beazley/refs/heads/main/openapi/beazley-products-api-openapi.yml
- filename: beazley-providers-api-openapi.yml
  format: yaml
  label: Beazley Providers API
  slug: beazley-providers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/beazley/refs/heads/main/openapi/beazley-providers-api-openapi.yml
- filename: beazley-rates-api-openapi.yml
  format: yaml
  label: Beazley Rates API
  slug: beazley-rates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/beazley/refs/heads/main/openapi/beazley-rates-api-openapi.yml
- filename: beazley-report-api-openapi.yml
  format: yaml
  label: Beazley Report API
  slug: beazley-report-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/beazley/refs/heads/main/openapi/beazley-report-api-openapi.yml
- filename: beazley-risks-api-openapi.yml
  format: yaml
  label: Beazley Risks API
  slug: beazley-risks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/beazley/refs/heads/main/openapi/beazley-risks-api-openapi.yml
- filename: beazley-search-api-openapi.yml
  format: yaml
  label: Beazley Search API
  slug: beazley-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/beazley/refs/heads/main/openapi/beazley-search-api-openapi.yml
auth_types:
- apiKey
description: 'Every Beazley API is fronted by Azure API Management and secured with an APIM subscription key. The key travels either in the Ocp-Apim-Subscription-Key request header or as a subscription-key query parameter; both schemes are declared in all fourteen published OpenAPI documents and both are accepted at the top level of every operation. There is no OAuth 2.0, no OpenID Connect and no mutual TLS anywhere on the public surface: neither /.well-known/openid-configuration nor /.well-known/oauth-authorization-server is served on any Beazley host.'
kind: authentication
layout: security
method: searched
name: Beazley Authentication
name_suffix: Authentication
oauth_flows: []
overview: Beazley secures its APIs with apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Beazley
provider_slug: beazley
scheme_count: 2
schemes:
- in: header
  name: apiKeyHeader
  parameter: Ocp-Apim-Subscription-Key
  sources:
  - openapi/beazley-about-beazley-sandbox.yml
  - openapi/beazley-about-beazley.yml
  - openapi/beazley-broker-and-insured-marketing-data-v2-sandbox.yml
  - openapi/beazley-broker-and-insured-marketing-data-v2.yml
  - openapi/beazley-compliance-web-api.yml
  - openapi/beazley-currency-exchange-sandbox.yml
  - openapi/beazley-currency-exchange.yml
  - openapi/beazley-data-capture-quote-and-risk-data-sandbox.yml
  - openapi/beazley-data-capture-quote-and-risk-data-v2-sandbox.yml
  - openapi/beazley-data-capture-quote-and-risk-data-v2.yml
  - openapi/beazley-data-capture-quote-and-risk-data-v3-pre-release.yml
  - openapi/beazley-data-capture-quote-and-risk-data.yml
  - openapi/beazley-fast-reader.yml
  - openapi/beazley-simple-raters.yml
  type: apiKey
- in: query
  name: apiKeyQuery
  parameter: subscription-key
  sources:
  - openapi/beazley-about-beazley-sandbox.yml
  - openapi/beazley-about-beazley.yml
  - openapi/beazley-broker-and-insured-marketing-data-v2-sandbox.yml
  - openapi/beazley-broker-and-insured-marketing-data-v2.yml
  - openapi/beazley-compliance-web-api.yml
  - openapi/beazley-currency-exchange-sandbox.yml
  - openapi/beazley-currency-exchange.yml
  - openapi/beazley-data-capture-quote-and-risk-data-sandbox.yml
  - openapi/beazley-data-capture-quote-and-risk-data-v2-sandbox.yml
  - openapi/beazley-data-capture-quote-and-risk-data-v2.yml
  - openapi/beazley-data-capture-quote-and-risk-data-v3-pre-release.yml
  - openapi/beazley-data-capture-quote-and-risk-data.yml
  - openapi/beazley-fast-reader.yml
  - openapi/beazley-simple-raters.yml
  type: apiKey
slug: beazley-authentication
source_filename: beazley-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-25'\nmethod: searched\nsource: openapi/beazley-about-beazley-sandbox.yml, openapi/beazley-about-beazley.yml, openapi/beazley-broker-and-insured-marketing-data-v2-sandbox.yml,\n  openapi/beazley-broker-and-insured-marketing-data-v2.yml, openapi/beazley-compliance-web-api.yml, openapi/beazley-currency-exchange-sandbox.yml,\n  openapi/beazley-currency-exchange.yml, openapi/beazley-data-capture-quote-and-risk-data-sandbox.yml,\n  openapi/beazley-data-capture-quote-and-risk-data-v2-sandbox.yml, openapi/beazley-data-capture-quote-and-risk-data-v2.yml,\n  openapi/beazley-data-capture-quote-and-risk-data-v3-pre-release.yml, openapi/beazley-data-capture-quote-and-risk-data.yml\n  ...\ndocs: https://developer.beazley.com/products\nmodel: api-key\ndescription: 'Every Beazley API is fronted by Azure API Management and secured with an APIM subscription\n  key. The key travels either in the Ocp-Apim-Subscription-Key request header or as a subscription-key\n  query parameter;\
  \ both schemes are declared in all fourteen published OpenAPI documents and both are\n  accepted at the top level of every operation. There is no OAuth 2.0, no OpenID Connect and no mutual\n  TLS anywhere on the public surface: neither /.well-known/openid-configuration nor /.well-known/oauth-authorization-server\n  is served on any Beazley host.'\nobtaining_credentials:\n  self_serve_account: true\n  signup: https://developer.beazley.com/signup\n  signin: https://developer.beazley.com/signin\n  self_serve_key: false\n  approval_required: true\n  note: 'A developer account is self-serve — email and password, no partner SSO — and unlocks the full\n    catalog and every OpenAPI download. A usable key is not self-serve: all nine published APIM products\n    carry subscriptionRequired=true AND approvalRequired=true, and eight of nine cap subscriptionsLimit\n    at 1, so Beazley must approve each subscription before the gateway will answer.'\n  contact: ITArchitecture@Beazley.com\nevidence:\n\
  - source: https://api.beazley.com/about/v1/people\n  status: 401\n  detail: 'WWW-Authenticate: AzureApiManagementKey realm=\"https://api.beazley.com/about/v1\", name=\"Ocp-Apim-Subscription-Key\",\n    type=\"header\"'\n- source: https://beazley.management.azure-api.net/.../products?api-version=2022-04-01-preview\n  status: 200\n  detail: 'All nine published products: subscriptionRequired=true, approvalRequired=true.'\n- source: https://www.beazley.com/.well-known/openid-configuration\n  status: soft-404\n  detail: Falls through to the site 404 page; no OIDC metadata served.\nnot_supported:\n- oauth2\n- openIdConnect\n- mutualTLS\n- http basic\n- http bearer\n- jwt\nscopes:\n  supported: false\n  note: API-key auth with no scope surface; authorisation is per-product subscription, not per-scope.\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\n  - query\nschemes:\n- name: apiKeyHeader\n  type: apiKey\n  in: header\n  parameter: Ocp-Apim-Subscription-Key\n  sources:\n  - openapi/beazley-about-beazley-sandbox.yml\n\
  \  - openapi/beazley-about-beazley.yml\n  - openapi/beazley-broker-and-insured-marketing-data-v2-sandbox.yml\n  - openapi/beazley-broker-and-insured-marketing-data-v2.yml\n  - openapi/beazley-compliance-web-api.yml\n  - openapi/beazley-currency-exchange-sandbox.yml\n  - openapi/beazley-currency-exchange.yml\n  - openapi/beazley-data-capture-quote-and-risk-data-sandbox.yml\n  - openapi/beazley-data-capture-quote-and-risk-data-v2-sandbox.yml\n  - openapi/beazley-data-capture-quote-and-risk-data-v2.yml\n  - openapi/beazley-data-capture-quote-and-risk-data-v3-pre-release.yml\n  - openapi/beazley-data-capture-quote-and-risk-data.yml\n  - openapi/beazley-fast-reader.yml\n  - openapi/beazley-simple-raters.yml\n- name: apiKeyQuery\n  type: apiKey\n  in: query\n  parameter: subscription-key\n  sources:\n  - openapi/beazley-about-beazley-sandbox.yml\n  - openapi/beazley-about-beazley.yml\n  - openapi/beazley-broker-and-insured-marketing-data-v2-sandbox.yml\n  - openapi/beazley-broker-and-insured-marketing-data-v2.yml\n\
  \  - openapi/beazley-compliance-web-api.yml\n  - openapi/beazley-currency-exchange-sandbox.yml\n  - openapi/beazley-currency-exchange.yml\n  - openapi/beazley-data-capture-quote-and-risk-data-sandbox.yml\n  - openapi/beazley-data-capture-quote-and-risk-data-v2-sandbox.yml\n  - openapi/beazley-data-capture-quote-and-risk-data-v2.yml\n  - openapi/beazley-data-capture-quote-and-risk-data-v3-pre-release.yml\n  - openapi/beazley-data-capture-quote-and-risk-data.yml\n  - openapi/beazley-fast-reader.yml\n  - openapi/beazley-simple-raters.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/beazley/refs/heads/main/authentication/beazley-authentication.yml
summary_line: apiKey · 2 schemes
tags:
- Insurance
- United Kingdom
- Property and Casualty
- Cyber Insurance
- Specialty Insurance
- Lloyd's of London
- Underwriting
- Risk Data
- Brokers
- Carrier
---
