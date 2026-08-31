---
api_key_in:
- query
- header
api_specs:
- filename: abstract-api-avatars-api-openapi.yml
  format: yaml
  label: Abstract API Avatars API
  slug: abstract-api-avatars-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/abstract-api/refs/heads/main/openapi/abstract-api-avatars-api-openapi.yml
- filename: abstract-api-company-enrichment-api-openapi.yml
  format: yaml
  label: Abstract API Company Enrichment API
  slug: abstract-api-company-enrichment-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/abstract-api/refs/heads/main/openapi/abstract-api-company-enrichment-api-openapi.yml
- filename: abstract-api-email-reputation-api-openapi.yml
  format: yaml
  label: Abstract API Email Reputation API
  slug: abstract-api-email-reputation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/abstract-api/refs/heads/main/openapi/abstract-api-email-reputation-api-openapi.yml
- filename: abstract-api-exchange-rates-api-openapi.yml
  format: yaml
  label: Abstract API Exchange Rates API
  slug: abstract-api-exchange-rates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/abstract-api/refs/heads/main/openapi/abstract-api-exchange-rates-api-openapi.yml
- filename: abstract-api-iban-validation-api-openapi.yml
  format: yaml
  label: Abstract API IBAN Validation API
  slug: abstract-api-iban-validation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/abstract-api/refs/heads/main/openapi/abstract-api-iban-validation-api-openapi.yml
- filename: abstract-api-image-processing-api-openapi.yml
  format: yaml
  label: Abstract API Image Processing API
  slug: abstract-api-image-processing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/abstract-api/refs/heads/main/openapi/abstract-api-image-processing-api-openapi.yml
- filename: abstract-api-ip-geolocation-api-openapi.yml
  format: yaml
  label: Abstract API IP Geolocation API
  slug: abstract-api-ip-geolocation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/abstract-api/refs/heads/main/openapi/abstract-api-ip-geolocation-api-openapi.yml
- filename: abstract-api-ip-intelligence-api-openapi.yml
  format: yaml
  label: Abstract API IP Intelligence API
  slug: abstract-api-ip-intelligence-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/abstract-api/refs/heads/main/openapi/abstract-api-ip-intelligence-api-openapi.yml
- filename: abstract-api-phone-intelligence-api-openapi.yml
  format: yaml
  label: Abstract API Phone Intelligence API
  slug: abstract-api-phone-intelligence-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/abstract-api/refs/heads/main/openapi/abstract-api-phone-intelligence-api-openapi.yml
- filename: abstract-api-public-holidays-api-openapi.yml
  format: yaml
  label: Abstract API Public Holidays API
  slug: abstract-api-public-holidays-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/abstract-api/refs/heads/main/openapi/abstract-api-public-holidays-api-openapi.yml
- filename: abstract-api-timezones-api-openapi.yml
  format: yaml
  label: Abstract API Timezones API
  slug: abstract-api-timezones-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/abstract-api/refs/heads/main/openapi/abstract-api-timezones-api-openapi.yml
- filename: abstract-api-vat-validation-api-openapi.yml
  format: yaml
  label: Abstract API VAT Validation API
  slug: abstract-api-vat-validation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/abstract-api/refs/heads/main/openapi/abstract-api-vat-validation-api-openapi.yml
- filename: abstract-api-web-scraping-api-openapi.yml
  format: yaml
  label: Abstract API Web Scraping API
  slug: abstract-api-web-scraping-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/abstract-api/refs/heads/main/openapi/abstract-api-web-scraping-api-openapi.yml
- filename: abstract-api-website-screenshot-api-openapi.yml
  format: yaml
  label: Abstract API Website Screenshot API
  slug: abstract-api-website-screenshot-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/abstract-api/refs/heads/main/openapi/abstract-api-website-screenshot-api-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: searched
name: Abstract Api Authentication
name_suffix: Authentication
oauth_flows: []
overview: Abstract API secures its APIs with apiKey and http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Abstract API
provider_slug: abstract-api
scheme_count: 1
schemes:
- in: query
  name: apiKey
  parameter: api_key
  sources:
  - openapi/abstract-api-avatars-api-openapi.yml
  - openapi/abstract-api-company-enrichment-api-openapi.yml
  - openapi/abstract-api-email-reputation-api-openapi.yml
  - openapi/abstract-api-exchange-rates-api-openapi.yml
  - openapi/abstract-api-iban-validation-api-openapi.yml
  - openapi/abstract-api-image-processing-api-openapi.yml
  - openapi/abstract-api-ip-geolocation-api-openapi.yml
  - openapi/abstract-api-ip-intelligence-api-openapi.yml
  - openapi/abstract-api-phone-intelligence-api-openapi.yml
  - openapi/abstract-api-public-holidays-api-openapi.yml
  - openapi/abstract-api-timezones-api-openapi.yml
  - openapi/abstract-api-vat-validation-api-openapi.yml
  - openapi/abstract-api-web-scraping-api-openapi.yml
  - openapi/abstract-api-website-screenshot-api-openapi.yml
  type: apiKey
slug: abstract-api-authentication
source_filename: abstract-api-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-29'\nmethod: searched\nsource: https://docs.abstractapi.com/api/email-reputation.md (Authentication Methods), https://docs.abstractapi.com/.well-known/agent-skills/abstractapi/skill.md,\n  openapi/_original/*.openapi.yaml (provider-published), plus the derived securityScheme scan of openapi/*.yml\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - query\n  - header\n  note: 'The refined openapi/*.yml declare only the api_key QUERY parameter. The provider documents a\n    second, equivalent method the refined specs omit: the same key sent as Authorization: Bearer <key>.\n    The provider-published definitions at openapi/_original/ declare both. Captured here so the auth profile\n    is not a version behind the provider.'\nschemes:\n- name: apiKey\n  type: apiKey\n  in: query\n  parameter: api_key\n  sources:\n  - openapi/abstract-api-avatars-api-openapi.yml\n  - openapi/abstract-api-company-enrichment-api-openapi.yml\n  - openapi/abstract-api-email-reputation-api-openapi.yml\n\
  \  - openapi/abstract-api-exchange-rates-api-openapi.yml\n  - openapi/abstract-api-iban-validation-api-openapi.yml\n  - openapi/abstract-api-image-processing-api-openapi.yml\n  - openapi/abstract-api-ip-geolocation-api-openapi.yml\n  - openapi/abstract-api-ip-intelligence-api-openapi.yml\n  - openapi/abstract-api-phone-intelligence-api-openapi.yml\n  - openapi/abstract-api-public-holidays-api-openapi.yml\n  - openapi/abstract-api-timezones-api-openapi.yml\n  - openapi/abstract-api-vat-validation-api-openapi.yml\n  - openapi/abstract-api-web-scraping-api-openapi.yml\n  - openapi/abstract-api-website-screenshot-api-openapi.yml\ndocs: https://docs.abstractapi.com/api/email-reputation\nmethods:\n- name: api-key-query\n  type: apiKey\n  in: query\n  parameter: api_key\n  example: GET https://emailreputation.abstractapi.com/v1/?api_key=KEY&email=user@example.com\n  provider_guidance: Simplest; the provider warns it exposes the key in URLs and server logs.\n- name: bearer-token\n  type: http\n\
  \  scheme: bearer\n  in: header\n  parameter: Authorization\n  example: 'Authorization: Bearer KEY'\n  provider_guidance: Recommended for production. When used, omit api_key from the query string.\n  gotcha: Must be \"Bearer KEY\" — not a bare key and not \"ApiKey KEY\".\n- name: form-post\n  type: apiKey\n  in: formData\n  parameter: api_key\n  example: 'POST body: api_key=KEY&email=user@example.com'\n- name: json-post\n  type: http\n  scheme: bearer\n  in: header\n  parameter: Authorization\n  example: 'POST {\"email\":\"user@example.com\"} with Authorization: Bearer KEY'\n  gotcha: 'Content-Type: application/json is required or the body is read as form data and the parameter\n    is not detected.'\nkey_management:\n  scope: per-product\n  note: Every Abstract product issues its own key. A key from one product returns 401 against another.\n    Keys are created and rotated in the dashboard at https://app.abstractapi.com/.\n  rotation_policy_published: false\n  expiry: none documented\n\
  \  domain_whitelisting:\n    available: true\n    tiers: Starter and above\n    note: Listed as a plan feature on every product pricing table.\noauth:\n  supported: false\n  note: No OAuth or OIDC. /.well-known/oauth-authorization-server and /.well-known/openid-configuration\n    404 on every host probed 2026-08-29. No scopes/ artifact is emitted, correctly.\nmtls:\n  supported: false\nunauthenticated_surface:\n  present: false\n  note: Every product endpoint requires a key; an unauthenticated call returns 400 or 401.\nfailure_modes:\n- status: 401\n  cause: missing key, wrong key, or a key issued for a different Abstract product\n- status: 422\n  cause: valid key, plan quota exhausted\n- status: 429\n  cause: valid key, per-second ceiling exceeded\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/abstract-api/refs/heads/main/authentication/abstract-api-authentication.yml
summary_line: apiKey/http · 1 scheme
tags:
- Avatars
- Company Enrichment
- Contacts
- Currency
- Email Validation
- Exchange Rates
- IBAN Validation
- Image Processing
- IP Geolocation
- IP Intelligence
- Phone Validation
- Public Holidays
- Screenshots
- Timezones
- VAT Validation
- Web Scraping
---
