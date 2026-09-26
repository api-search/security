---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: firma-dev-company-api-openapi.yml
  format: yaml
  label: Firma.dev Company API
  slug: firma-dev-company-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/firma-dev/refs/heads/main/openapi/firma-dev-company-api-openapi.yml
- filename: firma-dev-custom-fields-api-openapi.yml
  format: yaml
  label: Firma.dev Custom Fields API
  slug: firma-dev-custom-fields-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/firma-dev/refs/heads/main/openapi/firma-dev-custom-fields-api-openapi.yml
- filename: firma-dev-email-domains-api-openapi.yml
  format: yaml
  label: Firma.dev Email Domains API
  slug: firma-dev-email-domains-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/firma-dev/refs/heads/main/openapi/firma-dev-email-domains-api-openapi.yml
- filename: firma-dev-email-templates-api-openapi.yml
  format: yaml
  label: Firma.dev Email Templates API
  slug: firma-dev-email-templates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/firma-dev/refs/heads/main/openapi/firma-dev-email-templates-api-openapi.yml
- filename: firma-dev-jwt-management-api-openapi.yml
  format: yaml
  label: Firma.dev JWT Management API
  slug: firma-dev-jwt-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/firma-dev/refs/heads/main/openapi/firma-dev-jwt-management-api-openapi.yml
- filename: firma-dev-organization-seals-api-openapi.yml
  format: yaml
  label: Firma.dev Organization Seals API
  slug: firma-dev-organization-seals-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/firma-dev/refs/heads/main/openapi/firma-dev-organization-seals-api-openapi.yml
- filename: firma-dev-signer-terms-api-openapi.yml
  format: yaml
  label: Firma.dev Signer Terms API
  slug: firma-dev-signer-terms-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/firma-dev/refs/heads/main/openapi/firma-dev-signer-terms-api-openapi.yml
- filename: firma-dev-signing-requests-api-openapi.yml
  format: yaml
  label: Firma.dev Signing Requests API
  slug: firma-dev-signing-requests-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/firma-dev/refs/heads/main/openapi/firma-dev-signing-requests-api-openapi.yml
- filename: firma-dev-templates-api-openapi.yml
  format: yaml
  label: Firma.dev Templates API
  slug: firma-dev-templates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/firma-dev/refs/heads/main/openapi/firma-dev-templates-api-openapi.yml
- filename: firma-dev-webhooks-api-openapi.yml
  format: yaml
  label: Firma.dev Webhooks API
  slug: firma-dev-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/firma-dev/refs/heads/main/openapi/firma-dev-webhooks-api-openapi.yml
- filename: firma-dev-workspace-settings-api-openapi.yml
  format: yaml
  label: Firma.dev Workspace Settings API
  slug: firma-dev-workspace-settings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/firma-dev/refs/heads/main/openapi/firma-dev-workspace-settings-api-openapi.yml
- filename: firma-dev-workspaces-api-openapi.yml
  format: yaml
  label: Firma.dev Workspaces API
  slug: firma-dev-workspaces-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/firma-dev/refs/heads/main/openapi/firma-dev-workspaces-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Firma Dev Authentication
name_suffix: Authentication
oauth_flows: []
overview: Firma.dev secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Firma.dev
provider_slug: firma-dev
scheme_count: 1
schemes:
- description: API key for authentication. Use your API key directly without any prefix (e.g., 'your-api-key'). Bearer prefix is optional but not required.
  in: header
  name: ApiKeyAuth
  parameter: Authorization
  sources:
  - openapi/app_firma_dev_openapi.json
  type: apiKey
slug: firma-dev-authentication
source_filename: firma-dev-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-25'\nmethod: derived\nsource: openapi/app_firma_dev_openapi.json\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: API key for authentication. Use your API key directly without any prefix (e.g.,\n    'your-api-key'). Bearer prefix is optional but not required.\n  sources:\n  - openapi/app_firma_dev_openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/firma-dev/refs/heads/main/authentication/firma-dev-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- eSignature
- API
- DeveloperTools
- LowCost
- WhiteLabel
---
