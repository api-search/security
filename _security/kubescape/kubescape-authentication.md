---
api_key_in: []
api_specs:
- filename: kubescape-openapi.yml
  format: yaml
  label: Kubescape Posture & Compliance API
  slug: kubescape-posture-compliance-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kubescape/refs/heads/main/openapi/kubescape-openapi.yml
- filename: kubescape-openapi.yml
  format: yaml
  label: Kubescape Vulnerabilities API
  slug: kubescape-vulnerabilities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kubescape/refs/heads/main/openapi/kubescape-openapi.yml
- filename: kubescape-openapi.yml
  format: yaml
  label: Kubescape Runtime Security API
  slug: kubescape-runtime-security-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kubescape/refs/heads/main/openapi/kubescape-openapi.yml
- filename: kubescape-openapi.yml
  format: yaml
  label: Kubescape Network Policies API
  slug: kubescape-network-policies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kubescape/refs/heads/main/openapi/kubescape-openapi.yml
- filename: kubescape-openapi.yml
  format: yaml
  label: Kubescape Registry & Repository Scanning API
  slug: kubescape-registry-repository-scanning-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kubescape/refs/heads/main/openapi/kubescape-openapi.yml
- filename: kubescape-openapi.yml
  format: yaml
  label: Kubescape Access Keys API
  slug: kubescape-access-keys-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kubescape/refs/heads/main/openapi/kubescape-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Kubescape Authentication
name_suffix: Authentication
oauth_flows: []
overview: Kubescape secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Kubescape
provider_slug: kubescape
scheme_count: 1
schemes:
- description: ARMO Platform Customer API requests are authenticated with an Agent Access Key generated in ARMO Platform under Settings > Agent Access Keys, sent in the `X-API-KEY` request header. OAuth2 / OpenID Connect login is used for interactive console sessions. The open-source Kubescape CLI authenticates to ARMO for result submission with an account/access key via `kubescape scan --server api.armosec.io`; the in-cluster Operator component APIs are reachable inside the cluster and are not exposed publicly.
  in: header
  keyName: X-API-KEY
  name: apiKeyAuth
  sources:
  - https://hub.armosec.io/docs/authentication
  - openapi/kubescape-openapi.yml
  type: apiKey
slug: kubescape-authentication
source_filename: kubescape-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/kubescape-openapi.yml\nsummary:\n  types:\n  - apiKey\nschemes:\n- name: apiKeyAuth\n  type: apiKey\n  in: header\n  keyName: X-API-KEY\n  description: >-\n    ARMO Platform Customer API requests are authenticated with an Agent Access\n    Key generated in ARMO Platform under Settings > Agent Access Keys, sent in\n    the `X-API-KEY` request header. OAuth2 / OpenID Connect login is used for\n    interactive console sessions. The open-source Kubescape CLI authenticates to\n    ARMO for result submission with an account/access key via\n    `kubescape scan --server api.armosec.io`; the in-cluster Operator component\n    APIs are reachable inside the cluster and are not exposed publicly.\n  sources:\n  - https://hub.armosec.io/docs/authentication\n  - openapi/kubescape-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/kubescape/refs/heads/main/authentication/kubescape-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Kubernetes Security
- Cloud Native Security
- Container Security
- DevSecOps
- Kubernetes
- Vulnerability Scanning
- Compliance
- Runtime Security
- CNCF
- Open Source
---
