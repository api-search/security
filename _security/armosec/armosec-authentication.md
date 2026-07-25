---
api_key_in: []
api_specs:
- filename: armosec-access-keys-api-openapi.yml
  format: yaml
  label: ARMO Access Keys API
  slug: armosec-access-keys-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/armosec/refs/heads/main/openapi/armosec-access-keys-api-openapi.yml
- filename: armosec-clusters-api-openapi.yml
  format: yaml
  label: ARMO Clusters API
  slug: armosec-clusters-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/armosec/refs/heads/main/openapi/armosec-clusters-api-openapi.yml
- filename: armosec-integrations-api-openapi.yml
  format: yaml
  label: ARMO Integrations API
  slug: armosec-integrations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/armosec/refs/heads/main/openapi/armosec-integrations-api-openapi.yml
- filename: armosec-posture-api-openapi.yml
  format: yaml
  label: ARMO Posture API
  slug: armosec-posture-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/armosec/refs/heads/main/openapi/armosec-posture-api-openapi.yml
- filename: armosec-registry-api-openapi.yml
  format: yaml
  label: ARMO Registry API
  slug: armosec-registry-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/armosec/refs/heads/main/openapi/armosec-registry-api-openapi.yml
- filename: armosec-runtime-api-openapi.yml
  format: yaml
  label: ARMO Runtime API
  slug: armosec-runtime-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/armosec/refs/heads/main/openapi/armosec-runtime-api-openapi.yml
- filename: armosec-security-risks-api-openapi.yml
  format: yaml
  label: ARMO Security Risks API
  slug: armosec-security-risks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/armosec/refs/heads/main/openapi/armosec-security-risks-api-openapi.yml
- filename: armosec-vulnerabilities-api-openapi.yml
  format: yaml
  label: ARMO Vulnerabilities API
  slug: armosec-vulnerabilities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/armosec/refs/heads/main/openapi/armosec-vulnerabilities-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Armosec Authentication
name_suffix: Authentication
oauth_flows: []
overview: ARMO secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: ARMO
provider_slug: armosec
scheme_count: 1
schemes:
- description: ARMO Platform authenticates API calls with an account access key (Agent Access Key) generated in the platform under Settings > Agent Access Keys. The key is sent in the X-API-KEY request header. A session-cookie / OAuth2 (OpenID) login flow also exists for the web console, but access keys are the preferred way to authenticate programmatic API calls.
  in: header
  name: apiKeyAuth
  parameterName: X-API-KEY
  sources:
  - openapi/armosec-openapi.yml
  - https://hub.armosec.io/docs/armo-swagger-api
  type: apiKey
slug: armosec-authentication
source_filename: armosec-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/armosec-openapi.yml\nsummary:\n  types:\n  - apiKey\nschemes:\n- name: apiKeyAuth\n  type: apiKey\n  in: header\n  parameterName: X-API-KEY\n  description: >-\n    ARMO Platform authenticates API calls with an account access key (Agent\n    Access Key) generated in the platform under Settings > Agent Access Keys.\n    The key is sent in the X-API-KEY request header. A session-cookie / OAuth2\n    (OpenID) login flow also exists for the web console, but access keys are the\n    preferred way to authenticate programmatic API calls.\n  sources:\n  - openapi/armosec-openapi.yml\n  - https://hub.armosec.io/docs/armo-swagger-api\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/armosec/refs/heads/main/authentication/armosec-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Kubernetes Security
- Cloud Native Security
- CNAPP
- DevSecOps
- KSPM
- Vulnerability Management
- Compliance
- Runtime Security
- CADR
- Kubescape
- Container Security
---
