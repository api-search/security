---
api_key_in:
- header
api_specs:
- filename: dotfile-cases-openapi.yml
  format: yaml
  label: Dotfile API
  slug: dotfile-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dotfile/refs/heads/main/openapi/dotfile-cases-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Dotfile Authentication
name_suffix: Authentication
oauth_flows: []
overview: Dotfile secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Dotfile
provider_slug: dotfile
scheme_count: 1
schemes:
- description: Configure your api key in the Workspace settings
  in: header
  name: DotfileAPIKey
  parameter: X-DOTFILE-API-KEY
  sources:
  - openapi/dotfile-activities-openapi.yml
  - openapi/dotfile-aml-check-openapi.yml
  - openapi/dotfile-cases-openapi.yml
  - openapi/dotfile-checks-openapi.yml
  - openapi/dotfile-client-portal-openapi.yml
  - openapi/dotfile-companies-openapi.yml
  - openapi/dotfile-company-data-openapi.yml
  - openapi/dotfile-company-monitoring-check-openapi.yml
  - openapi/dotfile-custom-properties-openapi.yml
  - openapi/dotfile-document-check-openapi.yml
  - openapi/dotfile-ekyc-check-openapi.yml
  - openapi/dotfile-electronic-signature-check-openapi.yml
  - openapi/dotfile-files-openapi.yml
  - openapi/dotfile-fraud-database-check-openapi.yml
  - openapi/dotfile-id-document-check-openapi.yml
  - openapi/dotfile-id-verification-check-openapi.yml
  - openapi/dotfile-individuals-openapi.yml
  - openapi/dotfile-notes-openapi.yml
  - openapi/dotfile-online-reputation-check-openapi.yml
  - openapi/dotfile-ping-openapi.yml
  - openapi/dotfile-routines-openapi.yml
  - openapi/dotfile-tables-openapi.yml
  - openapi/dotfile-tags-openapi.yml
  - openapi/dotfile-templates-openapi.yml
  - openapi/dotfile-users-openapi.yml
  - openapi/dotfile-webhooks-openapi.yml
  type: apiKey
slug: dotfile-authentication
source_filename: dotfile-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-17'\nmethod: derived\nsource: openapi/dotfile-activities-openapi.yml, openapi/dotfile-aml-check-openapi.yml, openapi/dotfile-cases-openapi.yml,\n  openapi/dotfile-checks-openapi.yml, openapi/dotfile-client-portal-openapi.yml, openapi/dotfile-companies-openapi.yml,\n  openapi/dotfile-company-data-openapi.yml, openapi/dotfile-company-monitoring-check-openapi.yml,\n  openapi/dotfile-custom-properties-openapi.yml, openapi/dotfile-document-check-openapi.yml,\n  openapi/dotfile-ekyc-check-openapi.yml, openapi/dotfile-electronic-signature-check-openapi.yml\n  ...\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: DotfileAPIKey\n  type: apiKey\n  in: header\n  parameter: X-DOTFILE-API-KEY\n  description: Configure your api key in the Workspace settings\n  sources:\n  - openapi/dotfile-activities-openapi.yml\n  - openapi/dotfile-aml-check-openapi.yml\n  - openapi/dotfile-cases-openapi.yml\n  - openapi/dotfile-checks-openapi.yml\n  - openapi/dotfile-client-portal-openapi.yml\n\
  \  - openapi/dotfile-companies-openapi.yml\n  - openapi/dotfile-company-data-openapi.yml\n  - openapi/dotfile-company-monitoring-check-openapi.yml\n  - openapi/dotfile-custom-properties-openapi.yml\n  - openapi/dotfile-document-check-openapi.yml\n  - openapi/dotfile-ekyc-check-openapi.yml\n  - openapi/dotfile-electronic-signature-check-openapi.yml\n  - openapi/dotfile-files-openapi.yml\n  - openapi/dotfile-fraud-database-check-openapi.yml\n  - openapi/dotfile-id-document-check-openapi.yml\n  - openapi/dotfile-id-verification-check-openapi.yml\n  - openapi/dotfile-individuals-openapi.yml\n  - openapi/dotfile-notes-openapi.yml\n  - openapi/dotfile-online-reputation-check-openapi.yml\n  - openapi/dotfile-ping-openapi.yml\n  - openapi/dotfile-routines-openapi.yml\n  - openapi/dotfile-tables-openapi.yml\n  - openapi/dotfile-tags-openapi.yml\n  - openapi/dotfile-templates-openapi.yml\n  - openapi/dotfile-users-openapi.yml\n  - openapi/dotfile-webhooks-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/dotfile/refs/heads/main/authentication/dotfile-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- kyb
- kyc
- aml
- business-verification
- identity-verification
- compliance
- regtech
- onboarding
- sanctions-screening
- document-verification
- fraud-detection
- company-data
- beneficial-ownership
- case-management
- electronic-signature
- webhooks
---
