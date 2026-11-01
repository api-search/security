---
anonymous_access: false
api_key_in: []
api_specs:
- filename: honkio-ca-accounts-api-openapi.yml
  format: yaml
  label: honkio-ca Accounts API
  slug: honkio-ca-accounts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/honkio-ca/openapi/honkio-ca-accounts-api-openapi.yml
- filename: honkio-ca-auth-api-openapi.yml
  format: yaml
  label: honkio-ca Auth API
  slug: honkio-ca-auth-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/honkio-ca/openapi/honkio-ca-auth-api-openapi.yml
- filename: honkio-ca-compliance-casl-api-openapi.yml
  format: yaml
  label: honkio-ca Compliance / CASL API
  slug: honkio-ca-compliance-casl-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/honkio-ca/openapi/honkio-ca-compliance-casl-api-openapi.yml
- filename: honkio-ca-compliance-dncl-api-openapi.yml
  format: yaml
  label: honkio-ca Compliance / DNCL API
  slug: honkio-ca-compliance-dncl-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/honkio-ca/openapi/honkio-ca-compliance-dncl-api-openapi.yml
- filename: honkio-ca-compliance-pipeda-api-openapi.yml
  format: yaml
  label: honkio-ca Compliance / PIPEDA API
  slug: honkio-ca-compliance-pipeda-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/honkio-ca/openapi/honkio-ca-compliance-pipeda-api-openapi.yml
- filename: honkio-ca-contact-groups-api-openapi.yml
  format: yaml
  label: honkio-ca Contact Groups API
  slug: honkio-ca-contact-groups-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/honkio-ca/openapi/honkio-ca-contact-groups-api-openapi.yml
- filename: honkio-ca-contacts-api-openapi.yml
  format: yaml
  label: honkio-ca Contacts API
  slug: honkio-ca-contacts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/honkio-ca/openapi/honkio-ca-contacts-api-openapi.yml
- filename: honkio-ca-email-domains-api-openapi.yml
  format: yaml
  label: honkio-ca Email Domains API
  slug: honkio-ca-email-domains-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/honkio-ca/openapi/honkio-ca-email-domains-api-openapi.yml
- filename: honkio-ca-email-suppressions-api-openapi.yml
  format: yaml
  label: honkio-ca Email Suppressions API
  slug: honkio-ca-email-suppressions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/honkio-ca/openapi/honkio-ca-email-suppressions-api-openapi.yml
- filename: honkio-ca-email-templates-api-openapi.yml
  format: yaml
  label: honkio-ca Email Templates API
  slug: honkio-ca-email-templates-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/honkio-ca/openapi/honkio-ca-email-templates-api-openapi.yml
- filename: honkio-ca-emails-api-openapi.yml
  format: yaml
  label: honkio-ca Emails API
  slug: honkio-ca-emails-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/honkio-ca/openapi/honkio-ca-emails-api-openapi.yml
- filename: honkio-ca-lists-api-openapi.yml
  format: yaml
  label: honkio-ca Lists API
  slug: honkio-ca-lists-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/honkio-ca/openapi/honkio-ca-lists-api-openapi.yml
- filename: honkio-ca-messages-api-openapi.yml
  format: yaml
  label: honkio-ca Messages API
  slug: honkio-ca-messages-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/honkio-ca/openapi/honkio-ca-messages-api-openapi.yml
- filename: honkio-ca-oauth-api-openapi.yml
  format: yaml
  label: honkio-ca OAuth API
  slug: honkio-ca-oauth-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/honkio-ca/openapi/honkio-ca-oauth-api-openapi.yml
- filename: honkio-ca-phone-numbers-api-openapi.yml
  format: yaml
  label: honkio-ca Phone Numbers API
  slug: honkio-ca-phone-numbers-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/honkio-ca/openapi/honkio-ca-phone-numbers-api-openapi.yml
- filename: honkio-ca-pricing-api-openapi.yml
  format: yaml
  label: honkio-ca Pricing API
  slug: honkio-ca-pricing-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/honkio-ca/openapi/honkio-ca-pricing-api-openapi.yml
- filename: honkio-ca-verify-api-openapi.yml
  format: yaml
  label: honkio-ca Verify API
  slug: honkio-ca-verify-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/honkio-ca/openapi/honkio-ca-verify-api-openapi.yml
- filename: honkio-ca-webhooks-api-openapi.yml
  format: yaml
  label: honkio-ca Webhooks API
  slug: honkio-ca-webhooks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/honkio-ca/openapi/honkio-ca-webhooks-api-openapi.yml
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Honkio Ca Authentication
name_suffix: Authentication
oauth_flows: []
overview: honkio-ca declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: honkio-ca
provider_slug: honkio-ca
scheme_count: 2
schemes:
- description: 'Authorization: Bearer mk_live_...'
  scheme: bearer
  type: http
- description: 'X-API-Key: mk_live_...'
  in: header
  name: X-API-Key
  type: apiKey
slug: honkio-ca-authentication
source_filename: honkio-ca-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: searched\nsource: llms.txt\nschemes:\n  - type: http\n    scheme: bearer\n    description: \"Authorization: Bearer mk_live_...\"\n  - type: apiKey\n    in: header\n    name: X-API-Key\n    description: \"X-API-Key: mk_live_...\"\n"
source_yaml_url: https://artifacts.apis.io/honkio-ca/authentication/honkio-ca-authentication.yml
summary_line: 2 schemes
tags:
- SMS
- Email
- Canada
- CASL
- PIPEDA
- Company
---
