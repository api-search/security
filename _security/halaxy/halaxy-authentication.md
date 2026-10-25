---
anonymous_access: false
api_key_in: []
api_specs:
- filename: halaxy-appointment-api-openapi.yml
  format: yaml
  label: Halaxy Appointment API
  slug: halaxy-appointment-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/halaxy/refs/heads/main/openapi/halaxy-appointment-api-openapi.yml
- filename: halaxy-chargeitemdefinition-api-openapi.yml
  format: yaml
  label: Halaxy Charge Item Definition API
  slug: halaxy-chargeitemdefinition-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/halaxy/refs/heads/main/openapi/halaxy-chargeitemdefinition-api-openapi.yml
- filename: halaxy-coverage-api-openapi.yml
  format: yaml
  label: Halaxy Coverage API
  slug: halaxy-coverage-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/halaxy/refs/heads/main/openapi/halaxy-coverage-api-openapi.yml
- filename: halaxy-invoice-api-openapi.yml
  format: yaml
  label: Halaxy Invoice API
  slug: halaxy-invoice-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/halaxy/refs/heads/main/openapi/halaxy-invoice-api-openapi.yml
- filename: halaxy-invoiceline-api-openapi.yml
  format: yaml
  label: Halaxy Invoice Line API
  slug: halaxy-invoiceline-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/halaxy/refs/heads/main/openapi/halaxy-invoiceline-api-openapi.yml
- filename: halaxy-organization-api-openapi.yml
  format: yaml
  label: Halaxy Organization API
  slug: halaxy-organization-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/halaxy/refs/heads/main/openapi/halaxy-organization-api-openapi.yml
- filename: halaxy-patient-api-openapi.yml
  format: yaml
  label: Halaxy Patient API
  slug: halaxy-patient-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/halaxy/refs/heads/main/openapi/halaxy-patient-api-openapi.yml
- filename: halaxy-paymenttransaction-api-openapi.yml
  format: yaml
  label: Halaxy Payment Transaction API
  slug: halaxy-paymenttransaction-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/halaxy/refs/heads/main/openapi/halaxy-paymenttransaction-api-openapi.yml
- filename: halaxy-practitioner-api-openapi.yml
  format: yaml
  label: Halaxy Practitioner API
  slug: halaxy-practitioner-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/halaxy/refs/heads/main/openapi/halaxy-practitioner-api-openapi.yml
- filename: halaxy-referral-api-openapi.yml
  format: yaml
  label: Halaxy Referral API
  slug: halaxy-referral-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/halaxy/refs/heads/main/openapi/halaxy-referral-api-openapi.yml
- filename: halaxy-referraldefinition-api-openapi.yml
  format: yaml
  label: Halaxy Referral Definition API
  slug: halaxy-referraldefinition-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/halaxy/refs/heads/main/openapi/halaxy-referraldefinition-api-openapi.yml
- filename: halaxy-schedule-api-openapi.yml
  format: yaml
  label: Halaxy Schedule API
  slug: halaxy-schedule-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/halaxy/refs/heads/main/openapi/halaxy-schedule-api-openapi.yml
- filename: halaxy-slot-api-openapi.yml
  format: yaml
  label: Halaxy Slot API
  slug: halaxy-slot-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/halaxy/refs/heads/main/openapi/halaxy-slot-api-openapi.yml
- filename: halaxy-capability-statement-api-openapi.yml
  format: yaml
  label: Halaxy Capability Statement API
  slug: halaxy-capability-statement-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/halaxy/refs/heads/main/openapi/halaxy-capability-statement-api-openapi.yml
- filename: halaxy-document-reference-api-openapi.yml
  format: yaml
  label: Halaxy Document Reference API
  slug: halaxy-document-reference-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/halaxy/refs/heads/main/openapi/halaxy-document-reference-api-openapi.yml
- filename: halaxy-healthcare-service-api-openapi.yml
  format: yaml
  label: Halaxy Healthcare Service API
  slug: halaxy-healthcare-service-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/halaxy/refs/heads/main/openapi/halaxy-healthcare-service-api-openapi.yml
- filename: halaxy-practitioner-role-api-openapi.yml
  format: yaml
  label: Halaxy Practitioner Role API
  slug: halaxy-practitioner-role-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/halaxy/refs/heads/main/openapi/halaxy-practitioner-role-api-openapi.yml
- filename: halaxy-search-parameter-api-openapi.yml
  format: yaml
  label: Halaxy Search Parameter API
  slug: halaxy-search-parameter-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/halaxy/refs/heads/main/openapi/halaxy-search-parameter-api-openapi.yml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Halaxy Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: Halaxy secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: Halaxy
provider_slug: halaxy
scheme_count: 1
schemes:
- credentials: Client ID and Client Secret, created as an API Key on the Halaxy developer page after purchasing the Halaxy API subscription in Add-ons.
  description: OAuth 2.0 client credentials Grant
  flows:
  - flow: clientCredentials
    scopes: 0
    tokenUrl: /main/oauth/token
    token_url_documented: https://au-api.halaxy.com/main/oauth/token
  name: oauth
  regional_hosts:
  - https://au-api.halaxy.com/main/
  - https://eu-api.halaxy.com/main/
  sources:
  - openapi/halaxy-api-openapi.yml
  - https://developers.halaxy.com/docs/authentication.md
  token_lifetime_note: The docs' sample response shows "expires_in":3600 while the callout says "Access tokens are valid for 15 minutes." Both are quoted as published; the docs are inconsistent.
  token_lifetime_text: Access tokens are valid for 15 minutes.
  token_request: 'JSON body {"grant_type": "client_credentials", "client_id", "client_secret"}, Content-Type application/json'
  token_response: '{"token_type":"Bearer","expires_in":3600,"access_token":"..."}'
  type: oauth2
  usage: 'Authorization: Bearer <YOUR ACCESS TOKEN>'
slug: halaxy-authentication
source_filename: halaxy-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-22'\nmethod: searched\nsource: https://developers.halaxy.com/docs/authentication.md\ndocs: https://developers.halaxy.com/docs/authentication.md\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - clientCredentials\nschemes:\n- name: oauth\n  type: oauth2\n  flows:\n  - flow: clientCredentials\n    tokenUrl: /main/oauth/token\n    token_url_documented: https://au-api.halaxy.com/main/oauth/token\n    scopes: 0\n  description: OAuth 2.0 client credentials Grant\n  credentials: Client ID and Client Secret, created as an API Key on the Halaxy developer page after purchasing the Halaxy API subscription in Add-ons.\n  token_request: 'JSON body {\"grant_type\": \"client_credentials\", \"client_id\", \"client_secret\"}, Content-Type application/json'\n  token_response: '{\"token_type\":\"Bearer\",\"expires_in\":3600,\"access_token\":\"...\"}'\n  token_lifetime_text: Access tokens are valid for 15 minutes.\n  token_lifetime_note: The docs' sample response shows\
  \ \"expires_in\":3600 while the callout says \"Access tokens are valid for 15 minutes.\" Both are quoted as published; the docs are inconsistent.\n  usage: 'Authorization: Bearer <YOUR ACCESS TOKEN>'\n  regional_hosts:\n  - https://au-api.halaxy.com/main/\n  - https://eu-api.halaxy.com/main/\n  sources:\n  - openapi/halaxy-api-openapi.yml\n  - https://developers.halaxy.com/docs/authentication.md\nclient_identification:\n  header: 'User-Agent: APP_VENDOR_NAME (APP_VENDOR_EMAIL)'\n  source: https://developers.halaxy.com/docs/authentication.md\naccess_control: Per-key access is configured in the Halaxy API Key Manager (Settings > Integrations > External); the docs publish no scope list.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/halaxy/refs/heads/main/authentication/halaxy-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Company
- Healthcare
- Practice Management
- FHIR
- Telehealth
- Appointments
- Billing
- Patients
---
