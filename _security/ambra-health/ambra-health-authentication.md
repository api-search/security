---
api_key_in:
- header
api_specs:
- filename: ambra-health-openapi.yml
  format: yaml
  label: Ambra Health Session API
  slug: ambra-health-session-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ambra-health/refs/heads/main/openapi/ambra-health-openapi.yml
- filename: ambra-health-openapi.yml
  format: yaml
  label: Ambra Health Studies API
  slug: ambra-health-studies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ambra-health/refs/heads/main/openapi/ambra-health-openapi.yml
- filename: ambra-health-openapi.yml
  format: yaml
  label: Ambra Health Patients API
  slug: ambra-health-patients-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ambra-health/refs/heads/main/openapi/ambra-health-openapi.yml
- filename: ambra-health-openapi.yml
  format: yaml
  label: Ambra Health Users API
  slug: ambra-health-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ambra-health/refs/heads/main/openapi/ambra-health-openapi.yml
- filename: ambra-health-openapi.yml
  format: yaml
  label: Ambra Health Groups API
  slug: ambra-health-groups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ambra-health/refs/heads/main/openapi/ambra-health-openapi.yml
- filename: ambra-health-openapi.yml
  format: yaml
  label: Ambra Health Accounts API
  slug: ambra-health-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ambra-health/refs/heads/main/openapi/ambra-health-openapi.yml
- filename: ambra-health-openapi.yml
  format: yaml
  label: Ambra Health Namespaces API
  slug: ambra-health-namespaces-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ambra-health/refs/heads/main/openapi/ambra-health-openapi.yml
- filename: ambra-health-openapi.yml
  format: yaml
  label: Ambra Health Sharing API
  slug: ambra-health-sharing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ambra-health/refs/heads/main/openapi/ambra-health-openapi.yml
- filename: ambra-health-openapi.yml
  format: yaml
  label: Ambra Health Storage and Images API
  slug: ambra-health-storage-images-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ambra-health/refs/heads/main/openapi/ambra-health-openapi.yml
- filename: ambra-health-openapi.yml
  format: yaml
  label: Ambra Health Webhooks API
  slug: ambra-health-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ambra-health/refs/heads/main/openapi/ambra-health-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Ambra Health Authentication
name_suffix: Authentication
oauth_flows: []
overview: Ambra Health secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Ambra Health
provider_slug: ambra-health
scheme_count: 1
schemes:
- description: Session id (sid) obtained from POST /session/login. Also accepted as the sid request parameter.
  in: header
  name: sessionId
  parameter: X-AmbraHealth-SID
  sources:
  - openapi/ambra-health-openapi.yml
  type: apiKey
slug: ambra-health-authentication
source_filename: ambra-health-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/ambra-health-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: sessionId\n  type: apiKey\n  in: header\n  parameter: X-AmbraHealth-SID\n  description: Session id (sid) obtained from POST /session/login. Also accepted as the sid\n    request parameter.\n  sources:\n  - openapi/ambra-health-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ambra-health/refs/heads/main/authentication/ambra-health-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Medical Imaging
- DICOM
- Healthcare
- PACS
- Image Exchange
- Interoperability
- VNA
- Cloud Imaging
---
