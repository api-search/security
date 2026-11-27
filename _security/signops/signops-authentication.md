---
anonymous_access: false
api_key_in: []
api_specs:
- filename: signops-approve-api-openapi.yml
  format: yaml
  label: SignOps Approve API
  slug: signops-approve-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/signops/openapi/signops-approve-api-openapi.yml
- filename: signops-approve-sdk-api-openapi.yml
  format: yaml
  label: SignOps Approve SDK API
  slug: signops-approve-sdk-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/signops/openapi/signops-approve-sdk-api-openapi.yml
- filename: signops-authenticator-api-openapi.yml
  format: yaml
  label: SignOps Authenticator API
  slug: signops-authenticator-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/signops/openapi/signops-authenticator-api-openapi.yml
- filename: signops-devices-api-openapi.yml
  format: yaml
  label: SignOps Devices API
  slug: signops-devices-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/signops/openapi/signops-devices-api-openapi.yml
- filename: signops-email-otp-api-openapi.yml
  format: yaml
  label: SignOps Email OTP API
  slug: signops-email-otp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/signops/openapi/signops-email-otp-api-openapi.yml
- filename: signops-inbox-api-openapi.yml
  format: yaml
  label: SignOps Inbox API
  slug: signops-inbox-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/signops/openapi/signops-inbox-api-openapi.yml
- filename: signops-live-activities-api-openapi.yml
  format: yaml
  label: SignOps Live Activities API
  slug: signops-live-activities-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/signops/openapi/signops-live-activities-api-openapi.yml
- filename: signops-passkeys-api-openapi.yml
  format: yaml
  label: SignOps Passkeys API
  slug: signops-passkeys-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/signops/openapi/signops-passkeys-api-openapi.yml
- filename: signops-passkeys-browser-api-openapi.yml
  format: yaml
  label: SignOps Passkeys browser API
  slug: signops-passkeys-browser-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/signops/openapi/signops-passkeys-browser-api-openapi.yml
- filename: signops-push-api-openapi.yml
  format: yaml
  label: SignOps Push API
  slug: signops-push-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/signops/openapi/signops-push-api-openapi.yml
- filename: signops-status-api-openapi.yml
  format: yaml
  label: SignOps Status API
  slug: signops-status-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/signops/openapi/signops-status-api-openapi.yml
- filename: signops-templates-api-openapi.yml
  format: yaml
  label: SignOps Templates API
  slug: signops-templates-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/signops/openapi/signops-templates-api-openapi.yml
- filename: signops-topics-api-openapi.yml
  format: yaml
  label: SignOps Topics API
  slug: signops-topics-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/signops/openapi/signops-topics-api-openapi.yml
- filename: signops-users-and-dpdp-api-openapi.yml
  format: yaml
  label: SignOps Users and DPDP API
  slug: signops-users-and-dpdp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/signops/openapi/signops-users-and-dpdp-api-openapi.yml
- filename: signops-verify-api-openapi.yml
  format: yaml
  label: SignOps Verify API
  slug: signops-verify-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/signops/openapi/signops-verify-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: SignOps Authentication
name_suffix: Authentication
oauth_flows: []
overview: SignOps secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: SignOps
provider_slug: signops
scheme_count: 1
schemes:
- description: sk_live_... or sk_test_..., on your server only.
  name: secretKey
  scheme: bearer
  sources:
  - openapi/signops-openapi.json
  type: http
slug: signops-authentication
source_filename: signops-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-08'\nmethod: derived\nsource: openapi/signops-openapi.json\nsummary:\n  types:\n  - http\nschemes:\n- name: secretKey\n  type: http\n  scheme: bearer\n  description: sk_live_... or sk_test_..., on your server only.\n  sources:\n  - openapi/signops-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/signops/authentication/signops-authentication.yml
summary_line: http · 1 scheme
tags:
- Authentication
- OTP
- Push Notifications
- Passkeys
---
