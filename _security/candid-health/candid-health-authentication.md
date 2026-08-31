---
api_key_in: []
api_specs:
- filename: candid-health-default-api-openapi.yml
  format: yaml
  label: Candid Health Default API
  slug: candid-health-default-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/candid-health/refs/heads/main/openapi/candid-health-default-api-openapi.yml
- filename: candid-health-diagnoses-api-openapi.yml
  format: yaml
  label: Candid Health Diagnoses API
  slug: candid-health-diagnoses-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/candid-health/refs/heads/main/openapi/candid-health-diagnoses-api-openapi.yml
- filename: candid-health-v1-api-openapi.yml
  format: yaml
  label: Candid Health V1 API
  slug: candid-health-v1-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/candid-health/refs/heads/main/openapi/candid-health-v1-api-openapi.yml
- filename: candid-health-v2-api-openapi.yml
  format: yaml
  label: Candid Health V2 API
  slug: candid-health-v2-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/candid-health/refs/heads/main/openapi/candid-health-v2-api-openapi.yml
- filename: candid-health-v3-api-openapi.yml
  format: yaml
  label: Candid Health V3 API
  slug: candid-health-v3-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/candid-health/refs/heads/main/openapi/candid-health-v3-api-openapi.yml
- filename: candid-health-v4-api-openapi.yml
  format: yaml
  label: Candid Health V4 API
  slug: candid-health-v4-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/candid-health/refs/heads/main/openapi/candid-health-v4-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Candid Health Authentication
name_suffix: Authentication
oauth_flows: []
overview: Candid Health secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Candid Health
provider_slug: candid-health
scheme_count: 1
schemes:
- bearerFormat: JWT
  description: 'OAuth bearer token obtained from POST /auth/v2/token. Send as `Authorization: Bearer <access_token>`.'
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/candid-health-auth-api-openapi.yml
  - openapi/candid-health-charge-capture-api-openapi.yml
  - openapi/candid-health-eligibility-api-openapi.yml
  - openapi/candid-health-encounters-api-openapi.yml
  - openapi/candid-health-events-api-openapi.yml
  - openapi/candid-health-fee-schedules-api-openapi.yml
  - openapi/candid-health-insurance-adjudications-api-openapi.yml
  - openapi/candid-health-payers-api-openapi.yml
  - openapi/candid-health-subpackage-auth-subpackage-auth-default-api-openapi.yml
  - openapi/candid-health-subpackage-billing-notes-subpackage-billing-notes-v2-api-openapi.yml
  - openapi/candid-health-subpackage-charge-capture-bundles-subpackage-charge-capture-bundles-v1-api-openapi.yml
  - openapi/candid-health-subpackage-charge-capture-subpackage-charge-capture-v1-api-openapi.yml
  - openapi/candid-health-subpackage-contracts-subpackage-contracts-v2-api-openapi.yml
  - openapi/candid-health-subpackage-contracts-subpackage-contracts-v3-api-openapi.yml
  - openapi/candid-health-subpackage-credentialing-subpackage-credentialing-v2-api-openapi.yml
  - openapi/candid-health-subpackage-custom-schemas-subpackage-custom-schemas-v1-api-openapi.yml
  - openapi/candid-health-subpackage-diagnoses-api-openapi.yml
  - openapi/candid-health-subpackage-eligibility-subpackage-eligibility-v2-api-openapi.yml
  - openapi/candid-health-subpackage-encounter-attachments-subpackage-encounter-attachments-v1-api-openapi.yml
  - openapi/candid-health-subpackage-encounter-providers-subpackage-encounter-providers-v2-api-openapi.yml
  - openapi/candid-health-subpackage-encounter-supplemental-information-subpackage-encounter-supplemental-information-v1-api-openapi.yml
  - openapi/candid-health-subpackage-encounters-subpackage-encounters-v4-api-openapi.yml
  - openapi/candid-health-subpackage-events-subpackage-events-v1-api-openapi.yml
  - openapi/candid-health-subpackage-exports-subpackage-exports-v3-api-openapi.yml
  - openapi/candid-health-subpackage-external-payment-account-config-subpackage-external-payment-account-config-v1-api-openapi.yml
  - openapi/candid-health-subpackage-fee-schedules-subpackage-fee-schedules-v3-api-openapi.yml
  - openapi/candid-health-subpackage-guarantor-subpackage-guarantor-v1-api-openapi.yml
  - openapi/candid-health-subpackage-health-care-code-information-subpackage-health-care-code-information-v1-api-openapi.yml
  - openapi/candid-health-subpackage-import-invoice-subpackage-import-invoice-v1-api-openapi.yml
  - openapi/candid-health-subpackage-insurance-adjudications-subpackage-insurance-adjudications-v1-api-openapi.yml
  - openapi/candid-health-subpackage-insurance-refunds-subpackage-insurance-refunds-v1-api-openapi.yml
  - openapi/candid-health-subpackage-medication-dispense-subpackage-medication-dispense-v1-api-openapi.yml
  - openapi/candid-health-subpackage-non-insurance-payer-payments-subpackage-non-insurance-payer-payments-v1-api-openapi.yml
  - openapi/candid-health-subpackage-non-insurance-payer-refunds-subpackage-non-insurance-payer-refunds-v1-api-openapi.yml
  - openapi/candid-health-subpackage-non-insurance-payers-subpackage-non-insurance-payers-v1-api-openapi.yml
  - openapi/candid-health-subpackage-organization-providers-subpackage-organization-providers-v3-api-openapi.yml
  - openapi/candid-health-subpackage-organization-service-facilities-subpackage-organization-service-facilities-v2-api-openapi.yml
  - openapi/candid-health-subpackage-patient-ar-subpackage-patient-ar-v1-api-openapi.yml
  - openapi/candid-health-subpackage-patient-payments-subpackage-patient-payments-v4-api-openapi.yml
  - openapi/candid-health-subpackage-patient-refunds-subpackage-patient-refunds-v1-api-openapi.yml
  - openapi/candid-health-subpackage-payer-plan-groups-subpackage-payer-plan-groups-v1-api-openapi.yml
  - openapi/candid-health-subpackage-payers-subpackage-payers-v3-api-openapi.yml
  - openapi/candid-health-subpackage-payers-subpackage-payers-v4-api-openapi.yml
  - openapi/candid-health-subpackage-pre-encounter-subpackage-pre-encounter-appointments-subpackage-pre-encounter-appointments-v1-api-openapi.yml
  - openapi/candid-health-subpackage-pre-encounter-subpackage-pre-encounter-coverages-subpackage-pre-encounter-coverages-v1-api-openapi.yml
  - openapi/candid-health-subpackage-pre-encounter-subpackage-pre-encounter-eligibilitychecks-subpackage-pre-encounter-eligibilitychecks-v1-api-openapi.yml
  - openapi/candid-health-subpackage-pre-encounter-subpackage-pre-encounter-images-subpackage-pre-encounter-images-v1-api-openapi.yml
  - openapi/candid-health-subpackage-pre-encounter-subpackage-pre-encounter-lists-subpackage-pre-encounter-lists-v1-api-openapi.yml
  - openapi/candid-health-subpackage-pre-encounter-subpackage-pre-encounter-notes-subpackage-pre-encounter-notes-v1-api-openapi.yml
  - openapi/candid-health-subpackage-pre-encounter-subpackage-pre-encounter-organizationexternalproviders-subpackage-pre-encounter-organizationexternalproviders-v1-api-openapi.yml
  - openapi/candid-health-subpackage-pre-encounter-subpackage-pre-encounter-patients-subpackage-pre-encounter-patients-v1-api-openapi.yml
  - openapi/candid-health-subpackage-pre-encounter-subpackage-pre-encounter-tags-subpackage-pre-encounter-tags-v1-api-openapi.yml
  - openapi/candid-health-subpackage-service-lines-subpackage-service-lines-v2-api-openapi.yml
  - openapi/candid-health-subpackage-superbills-subpackage-superbills-v1-api-openapi.yml
  - openapi/candid-health-subpackage-tasks-subpackage-tasks-v3-api-openapi.yml
  - openapi/candid-health-subpackage-write-offs-subpackage-write-offs-v1-api-openapi.yml
  type: http
slug: candid-health-authentication
source_filename: candid-health-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-15'\nmethod: derived\nsource: openapi/candid-health-auth-api-openapi.yml, openapi/candid-health-charge-capture-api-openapi.yml,\n  openapi/candid-health-eligibility-api-openapi.yml, openapi/candid-health-encounters-api-openapi.yml,\n  openapi/candid-health-events-api-openapi.yml, openapi/candid-health-fee-schedules-api-openapi.yml,\n  openapi/candid-health-insurance-adjudications-api-openapi.yml, openapi/candid-health-payers-api-openapi.yml,\n  openapi/candid-health-subpackage-auth-subpackage-auth-default-api-openapi.yml, openapi/candid-health-subpackage-billing-notes-subpackage-billing-notes-v2-api-openapi.yml,\n  openapi/candid-health-subpackage-charge-capture-bundles-subpackage-charge-capture-bundles-v1-api-openapi.yml,\n  openapi/candid-health-subpackage-charge-capture-subpackage-charge-capture-v1-api-openapi.yml\n  ...\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: 'OAuth\
  \ bearer token obtained from POST /auth/v2/token. Send as `Authorization:\n    Bearer <access_token>`.'\n  sources:\n  - openapi/candid-health-auth-api-openapi.yml\n  - openapi/candid-health-charge-capture-api-openapi.yml\n  - openapi/candid-health-eligibility-api-openapi.yml\n  - openapi/candid-health-encounters-api-openapi.yml\n  - openapi/candid-health-events-api-openapi.yml\n  - openapi/candid-health-fee-schedules-api-openapi.yml\n  - openapi/candid-health-insurance-adjudications-api-openapi.yml\n  - openapi/candid-health-payers-api-openapi.yml\n  - openapi/candid-health-subpackage-auth-subpackage-auth-default-api-openapi.yml\n  - openapi/candid-health-subpackage-billing-notes-subpackage-billing-notes-v2-api-openapi.yml\n  - openapi/candid-health-subpackage-charge-capture-bundles-subpackage-charge-capture-bundles-v1-api-openapi.yml\n  - openapi/candid-health-subpackage-charge-capture-subpackage-charge-capture-v1-api-openapi.yml\n  - openapi/candid-health-subpackage-contracts-subpackage-contracts-v2-api-openapi.yml\n\
  \  - openapi/candid-health-subpackage-contracts-subpackage-contracts-v3-api-openapi.yml\n  - openapi/candid-health-subpackage-credentialing-subpackage-credentialing-v2-api-openapi.yml\n  - openapi/candid-health-subpackage-custom-schemas-subpackage-custom-schemas-v1-api-openapi.yml\n  - openapi/candid-health-subpackage-diagnoses-api-openapi.yml\n  - openapi/candid-health-subpackage-eligibility-subpackage-eligibility-v2-api-openapi.yml\n  - openapi/candid-health-subpackage-encounter-attachments-subpackage-encounter-attachments-v1-api-openapi.yml\n  - openapi/candid-health-subpackage-encounter-providers-subpackage-encounter-providers-v2-api-openapi.yml\n  - openapi/candid-health-subpackage-encounter-supplemental-information-subpackage-encounter-supplemental-information-v1-api-openapi.yml\n  - openapi/candid-health-subpackage-encounters-subpackage-encounters-v4-api-openapi.yml\n  - openapi/candid-health-subpackage-events-subpackage-events-v1-api-openapi.yml\n  - openapi/candid-health-subpackage-exports-subpackage-exports-v3-api-openapi.yml\n\
  \  - openapi/candid-health-subpackage-external-payment-account-config-subpackage-external-payment-account-config-v1-api-openapi.yml\n  - openapi/candid-health-subpackage-fee-schedules-subpackage-fee-schedules-v3-api-openapi.yml\n  - openapi/candid-health-subpackage-guarantor-subpackage-guarantor-v1-api-openapi.yml\n  - openapi/candid-health-subpackage-health-care-code-information-subpackage-health-care-code-information-v1-api-openapi.yml\n  - openapi/candid-health-subpackage-import-invoice-subpackage-import-invoice-v1-api-openapi.yml\n  - openapi/candid-health-subpackage-insurance-adjudications-subpackage-insurance-adjudications-v1-api-openapi.yml\n  - openapi/candid-health-subpackage-insurance-refunds-subpackage-insurance-refunds-v1-api-openapi.yml\n  - openapi/candid-health-subpackage-medication-dispense-subpackage-medication-dispense-v1-api-openapi.yml\n  - openapi/candid-health-subpackage-non-insurance-payer-payments-subpackage-non-insurance-payer-payments-v1-api-openapi.yml\n  - openapi/candid-health-subpackage-non-insurance-payer-refunds-subpackage-non-insurance-payer-refunds-v1-api-openapi.yml\n\
  \  - openapi/candid-health-subpackage-non-insurance-payers-subpackage-non-insurance-payers-v1-api-openapi.yml\n  - openapi/candid-health-subpackage-organization-providers-subpackage-organization-providers-v3-api-openapi.yml\n  - openapi/candid-health-subpackage-organization-service-facilities-subpackage-organization-service-facilities-v2-api-openapi.yml\n  - openapi/candid-health-subpackage-patient-ar-subpackage-patient-ar-v1-api-openapi.yml\n  - openapi/candid-health-subpackage-patient-payments-subpackage-patient-payments-v4-api-openapi.yml\n  - openapi/candid-health-subpackage-patient-refunds-subpackage-patient-refunds-v1-api-openapi.yml\n  - openapi/candid-health-subpackage-payer-plan-groups-subpackage-payer-plan-groups-v1-api-openapi.yml\n  - openapi/candid-health-subpackage-payers-subpackage-payers-v3-api-openapi.yml\n  - openapi/candid-health-subpackage-payers-subpackage-payers-v4-api-openapi.yml\n  - openapi/candid-health-subpackage-pre-encounter-subpackage-pre-encounter-appointments-subpackage-pre-encounter-appointments-v1-api-openapi.yml\n\
  \  - openapi/candid-health-subpackage-pre-encounter-subpackage-pre-encounter-coverages-subpackage-pre-encounter-coverages-v1-api-openapi.yml\n  - openapi/candid-health-subpackage-pre-encounter-subpackage-pre-encounter-eligibilitychecks-subpackage-pre-encounter-eligibilitychecks-v1-api-openapi.yml\n  - openapi/candid-health-subpackage-pre-encounter-subpackage-pre-encounter-images-subpackage-pre-encounter-images-v1-api-openapi.yml\n  - openapi/candid-health-subpackage-pre-encounter-subpackage-pre-encounter-lists-subpackage-pre-encounter-lists-v1-api-openapi.yml\n  - openapi/candid-health-subpackage-pre-encounter-subpackage-pre-encounter-notes-subpackage-pre-encounter-notes-v1-api-openapi.yml\n  - openapi/candid-health-subpackage-pre-encounter-subpackage-pre-encounter-organizationexternalproviders-subpackage-pre-encounter-organizationexternalproviders-v1-api-openapi.yml\n  - openapi/candid-health-subpackage-pre-encounter-subpackage-pre-encounter-patients-subpackage-pre-encounter-patients-v1-api-openapi.yml\n\
  \  - openapi/candid-health-subpackage-pre-encounter-subpackage-pre-encounter-tags-subpackage-pre-encounter-tags-v1-api-openapi.yml\n  - openapi/candid-health-subpackage-service-lines-subpackage-service-lines-v2-api-openapi.yml\n  - openapi/candid-health-subpackage-superbills-subpackage-superbills-v1-api-openapi.yml\n  - openapi/candid-health-subpackage-tasks-subpackage-tasks-v3-api-openapi.yml\n  - openapi/candid-health-subpackage-write-offs-subpackage-write-offs-v1-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/candid-health/refs/heads/main/authentication/candid-health-authentication.yml
summary_line: http · 1 scheme
tags:
- Medical Billing
- Revenue Cycle Management
- Healthcare
- Claims
- Eligibility
- Prior Authorization
- Remittance
- Patient Collections
- Credentialing
- Insurance
---
