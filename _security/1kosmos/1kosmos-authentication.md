---
api_key_in:
- header
api_specs:
- filename: 1kosmos-access-code-api-openapi.yml
  format: yaml
  label: 1Kosmos Access Code API
  slug: 1kosmos-access-code-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/1kosmos/refs/heads/main/openapi/1kosmos-access-code-api-openapi.yml
- filename: 1kosmos-ial-api-openapi.yml
  format: yaml
  label: 1Kosmos IAL API
  slug: 1kosmos-ial-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/1kosmos/refs/heads/main/openapi/1kosmos-ial-api-openapi.yml
- filename: 1kosmos-ial2-api-openapi.yml
  format: yaml
  label: 1Kosmos IAL2 API
  slug: 1kosmos-ial2-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/1kosmos/refs/heads/main/openapi/1kosmos-ial2-api-openapi.yml
- filename: 1kosmos-id-verification-api-openapi.yml
  format: yaml
  label: 1Kosmos ID Verification API
  slug: 1kosmos-id-verification-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/1kosmos/refs/heads/main/openapi/1kosmos-id-verification-api-openapi.yml
- filename: 1kosmos-otp-api-openapi.yml
  format: yaml
  label: 1Kosmos OTP API
  slug: 1kosmos-otp-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/1kosmos/refs/heads/main/openapi/1kosmos-otp-api-openapi.yml
- filename: 1kosmos-reports-api-openapi.yml
  format: yaml
  label: 1Kosmos Reports API
  slug: 1kosmos-reports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/1kosmos/refs/heads/main/openapi/1kosmos-reports-api-openapi.yml
- filename: 1kosmos-set-up-api-openapi.yml
  format: yaml
  label: 1Kosmos Set up API
  slug: 1kosmos-set-up-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/1kosmos/refs/heads/main/openapi/1kosmos-set-up-api-openapi.yml
- filename: 1kosmos-user-management-api-openapi.yml
  format: yaml
  label: 1Kosmos User Management API
  slug: 1kosmos-user-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/1kosmos/refs/heads/main/openapi/1kosmos-user-management-api-openapi.yml
- filename: 1kosmos-verifiable-credentials-api-openapi.yml
  format: yaml
  label: 1Kosmos Verifiable Credentials API
  slug: 1kosmos-verifiable-credentials-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/1kosmos/refs/heads/main/openapi/1kosmos-verifiable-credentials-api-openapi.yml
- filename: 1kosmos-workflow-api-api-openapi.yml
  format: yaml
  label: 1Kosmos Workflow API API
  slug: 1kosmos-workflow-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/1kosmos/refs/heads/main/openapi/1kosmos-workflow-api-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: 1Kosmos Authentication
name_suffix: Authentication
oauth_flows: []
overview: 1Kosmos secures its APIs with apiKey across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: 1Kosmos
provider_slug: 1kosmos
scheme_count: 3
schemes:
- description: The tenant/community license key, ECDSA-encrypted with the shared secret derived from the caller private key and the community public key (see BIDECDSA in the first-party helper SDKs). Sent unencrypted only when the noecdsa header is set.
  in: header
  name: licenseKey
  parameter: licensekey
  sources:
  - openapi/1kosmos-blockid-openapi.yml
  type: apiKey
- description: The caller ECDSA public key, used by the service to derive the shared secret that decrypts licensekey and encrypted payloads.
  in: header
  name: publicKey
  parameter: publickey
  sources:
  - openapi/1kosmos-blockid-openapi.yml
  type: apiKey
- description: Tenant tag, required by the reports, user-management and access-code services.
  in: header
  name: tenantTag
  parameter: X-TenantTag
  sources:
  - openapi/1kosmos-blockid-openapi.yml
  type: apiKey
slug: 1kosmos-authentication
source_filename: 1kosmos-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-05'\nmethod: derived\nsource: openapi/1kosmos-blockid-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: licenseKey\n  type: apiKey\n  in: header\n  parameter: licensekey\n  description: The tenant/community license key, ECDSA-encrypted with the shared secret derived\n    from the caller private key and the community public key (see BIDECDSA in the first-party\n    helper SDKs). Sent unencrypted only when the noecdsa header is set.\n  sources:\n  - openapi/1kosmos-blockid-openapi.yml\n- name: publicKey\n  type: apiKey\n  in: header\n  parameter: publickey\n  description: The caller ECDSA public key, used by the service to derive the shared secret\n    that decrypts licensekey and encrypted payloads.\n  sources:\n  - openapi/1kosmos-blockid-openapi.yml\n- name: tenantTag\n  type: apiKey\n  in: header\n  parameter: X-TenantTag\n  description: Tenant tag, required by the reports, user-management and access-code services.\n\
  \  sources:\n  - openapi/1kosmos-blockid-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/1kosmos/refs/heads/main/authentication/1kosmos-authentication.yml
summary_line: apiKey · 3 schemes
tags:
- Identity
- Authentication
- Identity Verification
- Passwordless
- Biometrics
- Verifiable Credentials
- FIDO2
- Security
- Company
---
