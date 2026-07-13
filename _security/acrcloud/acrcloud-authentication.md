---
api_key_in:
- query
api_specs:
- filename: acrcloud-openapi.yml
  format: yaml
  label: ACRCloud Identification API
  slug: identification
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/acrcloud/refs/heads/main/openapi/acrcloud-openapi.yml
- filename: acrcloud-openapi.yml
  format: yaml
  label: ACRCloud File Scanning API
  slug: file-scanning
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/acrcloud/refs/heads/main/openapi/acrcloud-openapi.yml
- filename: acrcloud-openapi.yml
  format: yaml
  label: ACRCloud Broadcast Monitoring API
  slug: broadcast-monitoring
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/acrcloud/refs/heads/main/openapi/acrcloud-openapi.yml
- filename: acrcloud-openapi.yml
  format: yaml
  label: ACRCloud Buckets & Metadata API
  slug: buckets-metadata
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/acrcloud/refs/heads/main/openapi/acrcloud-openapi.yml
- filename: acrcloud-openapi.yml
  format: yaml
  label: ACRCloud Console API
  slug: console
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/acrcloud/refs/heads/main/openapi/acrcloud-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: derived
name: Acrcloud Authentication
name_suffix: Authentication
oauth_flows: []
overview: ACRCloud secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: ACRCloud
provider_slug: acrcloud
scheme_count: 2
schemes:
- description: HMAC-SHA1 request signing for the Identification API. The client sends access_key, timestamp, signature_version=1, data_type, and a Base64 signature. The signature is HMAC-SHA1 of the string "POST\n/v1/identify\n {access_key}\n{data_type}\n1\n{timestamp}" keyed with the access_secret.
  in: query
  name: acrSignature
  parameter: signature
  sources:
  - openapi/acrcloud-openapi.yml
  type: apiKey
- description: 'Console API access token created in the ACRCloud console developer settings and sent as "Authorization: Bearer {token}".'
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/acrcloud-openapi.yml
  type: http
slug: acrcloud-authentication
source_filename: acrcloud-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/acrcloud-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - query\nschemes:\n- name: acrSignature\n  type: apiKey\n  in: query\n  parameter: signature\n  description: HMAC-SHA1 request signing for the Identification API. The client sends access_key,\n    timestamp, signature_version=1, data_type, and a Base64 signature. The signature is HMAC-SHA1\n    of the string \"POST\\n/v1/identify\\n {access_key}\\n{data_type}\\n1\\n{timestamp}\" keyed with\n    the access_secret.\n  sources:\n  - openapi/acrcloud-openapi.yml\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: 'Console API access token created in the ACRCloud console developer settings\n    and sent as \"Authorization: Bearer {token}\".'\n  sources:\n  - openapi/acrcloud-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/acrcloud/refs/heads/main/authentication/acrcloud-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Audio
- Music Recognition
- Audio Fingerprinting
- Broadcast Monitoring
- Metadata
---
