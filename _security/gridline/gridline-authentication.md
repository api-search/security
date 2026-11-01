---
anonymous_access: false
api_key_in: []
api_specs:
- filename: gridline-deepfake-api-openapi.yml
  format: yaml
  label: Gridlines Deepfake API
  slug: gridline-deepfake-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/gridline/openapi/gridline-deepfake-api-openapi.yml
- filename: gridline-digilocker-api-openapi.yml
  format: yaml
  label: Gridlines Digilocker API
  slug: gridline-digilocker-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/gridline/openapi/gridline-digilocker-api-openapi.yml
- filename: gridline-e-sign-api-openapi.yml
  format: yaml
  label: Gridlines E Sign API
  slug: gridline-e-sign-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/gridline/openapi/gridline-e-sign-api-openapi.yml
- filename: gridline-face-api-api-openapi.yml
  format: yaml
  label: Gridlines Face API
  slug: gridline-face-api-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/gridline/openapi/gridline-face-api-api-openapi.yml
- filename: gridline-individual-api-openapi.yml
  format: yaml
  label: Gridlines Individual API
  slug: gridline-individual-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/gridline/openapi/gridline-individual-api-openapi.yml
- filename: gridline-liveness-api-openapi.yml
  format: yaml
  label: Gridlines Liveness API
  slug: gridline-liveness-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/gridline/openapi/gridline-liveness-api-openapi.yml
- filename: gridline-pull-education-documents-api-openapi.yml
  format: yaml
  label: Gridlines Pull Education Documents API
  slug: gridline-pull-education-documents-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/gridline/openapi/gridline-pull-education-documents-api-openapi.yml
- filename: gridline-uidai-ovse-api-openapi.yml
  format: yaml
  label: Gridlines UIDAI OVSE API
  slug: gridline-uidai-ovse-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/gridline/openapi/gridline-uidai-ovse-api-openapi.yml
- filename: gridline-utility-api-openapi.yml
  format: yaml
  label: Gridlines Utility API
  slug: gridline-utility-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/gridline/openapi/gridline-utility-api-openapi.yml
- filename: gridline-workflow-mgmt-api-openapi.yml
  format: yaml
  label: Gridlines Workflow Mgmt API
  slug: gridline-workflow-mgmt-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/gridline/openapi/gridline-workflow-mgmt-api-openapi.yml
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 3
method: searched
name: Gridline Authentication
name_suffix: Authentication
oauth_flows: []
overview: Gridlines declares 3 security scheme(s) across its OpenAPI definitions.
provider_name: Gridlines
provider_slug: gridline
scheme_count: 3
schemes:
- description: API key for authentication. Keys "carry many privileges" and must not be placed in client-side code.
  in: header
  name: X-API-Key
  type: apiKey
- description: Must be set to 'API-Key'.
  in: header
  name: X-Auth-Type
  type: apiKey
- description: SDK session token. Documented as POST /v1/auth/tokens with X-Auth-Type API-Key and the server-side X-API-Key, returning access_token, token_type 'Bearer', access_token_expires_in, refresh_token and refresh_token_expires_in. Documented only; not called by this pipeline.
  docs: https://gridlines.stoplight.io/docs/gridlines-api-docs/9e848f3922672-aadhaar-ovse-web-sdk-react-native-integration-guide
  scheme: bearer
  type: http
slug: gridline-authentication
source_filename: gridline-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-28'\nmethod: searched\nsource: https://gridlines.stoplight.io/\ndocs: https://gridlines.stoplight.io/\nsummary: API keys are generated in the Gridlines account after enabling an API; each key can be authorised for one or more Gridlines APIs. All requests must use HTTPS and carry the X-Auth-Type and X-API-Key headers. For the Aadhaar OVSE Web SDK, the client backend exchanges the server-side API key for a short-lived bearer session and passes only that token to the browser/app.\nschemes:\n  - type: apiKey\n    name: X-API-Key\n    in: header\n    description: API key for authentication. Keys \"carry many privileges\" and must not be placed in client-side code.\n  - type: apiKey\n    name: X-Auth-Type\n    in: header\n    description: Must be set to 'API-Key'.\n  - type: http\n    scheme: bearer\n    description: SDK session token. Documented as POST /v1/auth/tokens with X-Auth-Type API-Key and the server-side X-API-Key, returning access_token, token_type\
  \ 'Bearer', access_token_expires_in, refresh_token and refresh_token_expires_in. Documented only; not called by this pipeline.\n    docs: https://gridlines.stoplight.io/docs/gridlines-api-docs/9e848f3922672-aadhaar-ovse-web-sdk-react-native-integration-guide\nkey_management:\n  per_module_keys: true\n  note: \"You can choose to generate different API Keys for each of your modules invoking Gridlines APIs or you can choose to use a single API key across your account.\"\n"
source_yaml_url: https://artifacts.apis.io/gridline/authentication/gridline-authentication.yml
summary_line: 3 schemes
tags:
- Company
- Onboarding
- IdentityVerification
- KYC
- eSigning
- FraudDetection
- VideoKYC
- DigitalOnboarding
- Fintech
---
