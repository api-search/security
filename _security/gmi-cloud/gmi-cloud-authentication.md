---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: gmi-cloud-baremetals-api-openapi.yml
  format: yaml
  label: GMI Cloud Baremetals API
  slug: gmi-cloud-baremetals-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gmi-cloud/refs/heads/main/openapi/gmi-cloud-baremetals-api-openapi.yml
- filename: gmi-cloud-containers-api-openapi.yml
  format: yaml
  label: GMI Cloud Containers API
  slug: gmi-cloud-containers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gmi-cloud/refs/heads/main/openapi/gmi-cloud-containers-api-openapi.yml
- filename: gmi-cloud-elastic-ips-api-openapi.yml
  format: yaml
  label: GMI Cloud Elastic Ips API
  slug: gmi-cloud-elastic-ips-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gmi-cloud/refs/heads/main/openapi/gmi-cloud-elastic-ips-api-openapi.yml
- filename: gmi-cloud-firewalls-api-openapi.yml
  format: yaml
  label: GMI Cloud Firewalls API
  slug: gmi-cloud-firewalls-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gmi-cloud/refs/heads/main/openapi/gmi-cloud-firewalls-api-openapi.yml
- filename: gmi-cloud-idcs-api-openapi.yml
  format: yaml
  label: GMI Cloud Idcs API
  slug: gmi-cloud-idcs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gmi-cloud/refs/heads/main/openapi/gmi-cloud-idcs-api-openapi.yml
- filename: gmi-cloud-images-api-openapi.yml
  format: yaml
  label: GMI Cloud Images API
  slug: gmi-cloud-images-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gmi-cloud/refs/heads/main/openapi/gmi-cloud-images-api-openapi.yml
- filename: gmi-cloud-invitations-api-openapi.yml
  format: yaml
  label: GMI Cloud Invitations API
  slug: gmi-cloud-invitations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gmi-cloud/refs/heads/main/openapi/gmi-cloud-invitations-api-openapi.yml
- filename: gmi-cloud-logs-api-openapi.yml
  format: yaml
  label: GMI Cloud Logs API
  slug: gmi-cloud-logs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gmi-cloud/refs/heads/main/openapi/gmi-cloud-logs-api-openapi.yml
- filename: gmi-cloud-me-api-openapi.yml
  format: yaml
  label: GMI Cloud Me API
  slug: gmi-cloud-me-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gmi-cloud/refs/heads/main/openapi/gmi-cloud-me-api-openapi.yml
- filename: gmi-cloud-oauth-api-openapi.yml
  format: yaml
  label: GMI Cloud OAuth API
  slug: gmi-cloud-oauth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gmi-cloud/refs/heads/main/openapi/gmi-cloud-oauth-api-openapi.yml
- filename: gmi-cloud-organizations-api-openapi.yml
  format: yaml
  label: GMI Cloud Organizations API
  slug: gmi-cloud-organizations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gmi-cloud/refs/heads/main/openapi/gmi-cloud-organizations-api-openapi.yml
- filename: gmi-cloud-sandbox-api-openapi.yml
  format: yaml
  label: GMI Cloud Sandbox API
  slug: gmi-cloud-sandbox-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gmi-cloud/refs/heads/main/openapi/gmi-cloud-sandbox-api-openapi.yml
- filename: gmi-cloud-sandbox-exec-api-openapi.yml
  format: yaml
  label: GMI Cloud Sandbox Exec API
  slug: gmi-cloud-sandbox-exec-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gmi-cloud/refs/heads/main/openapi/gmi-cloud-sandbox-exec-api-openapi.yml
- filename: gmi-cloud-sandbox-files-api-openapi.yml
  format: yaml
  label: GMI Cloud Sandbox Files API
  slug: gmi-cloud-sandbox-files-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gmi-cloud/refs/heads/main/openapi/gmi-cloud-sandbox-files-api-openapi.yml
- filename: gmi-cloud-sandboxtemplate-api-openapi.yml
  format: yaml
  label: GMI Cloud Sandbox Template API
  slug: gmi-cloud-sandboxtemplate-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gmi-cloud/refs/heads/main/openapi/gmi-cloud-sandboxtemplate-api-openapi.yml
- filename: gmi-cloud-templates-api-openapi.yml
  format: yaml
  label: GMI Cloud Templates API
  slug: gmi-cloud-templates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gmi-cloud/refs/heads/main/openapi/gmi-cloud-templates-api-openapi.yml
- filename: gmi-cloud-users-api-openapi.yml
  format: yaml
  label: GMI Cloud Users API
  slug: gmi-cloud-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gmi-cloud/refs/heads/main/openapi/gmi-cloud-users-api-openapi.yml
- filename: gmi-cloud-vpcs-api-openapi.yml
  format: yaml
  label: GMI Cloud Vpcs API
  slug: gmi-cloud-vpcs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gmi-cloud/refs/heads/main/openapi/gmi-cloud-vpcs-api-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: derived
name: Gmi Cloud Authentication
name_suffix: Authentication
oauth_flows: []
overview: GMI Cloud secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: GMI Cloud
provider_slug: gmi-cloud
scheme_count: 2
schemes:
- bearerFormat: JWT
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/gmi-cloud-cluster-engine-openapi.yml
  - openapi/gmi-cloud-idc-service-openapi.yml
  - openapi/gmi-cloud-sandbox-openapi.yml
  type: http
- description: 'Sandbox data-plane token — the `sandbox_access_token` returned by the create/connect endpoints. Used for `/files`, Sandbox-Exec, and other data-plane endpoints; the control plane (`/api/v2`) does not accept it, and conversely the control plane''s `Authorization: Bearer` is invalid on the data plane.


    The token is bound to its sandbox: using sandbox A''s token against sandbox B''s host fails. It stays'
  in: header
  name: sandboxAccessToken
  parameter: X-Access-Token
  sources:
  - openapi/gmi-cloud-sandbox-openapi.yml
  type: apiKey
slug: gmi-cloud-authentication
source_filename: gmi-cloud-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-13'\nmethod: derived\nsource: openapi/gmi-cloud-cluster-engine-openapi.yml, openapi/gmi-cloud-idc-service-openapi.yml,\n  openapi/gmi-cloud-sandbox-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  sources:\n  - openapi/gmi-cloud-cluster-engine-openapi.yml\n  - openapi/gmi-cloud-idc-service-openapi.yml\n  - openapi/gmi-cloud-sandbox-openapi.yml\n- name: sandboxAccessToken\n  type: apiKey\n  in: header\n  parameter: X-Access-Token\n  description: |-\n    Sandbox data-plane token — the `sandbox_access_token` returned by the create/connect endpoints. Used for `/files`, Sandbox-Exec, and other data-plane endpoints; the control plane (`/api/v2`) does not accept it, and conversely the control plane's `Authorization: Bearer` is invalid on the data plane.\n\n    The token is bound to its sandbox: using sandbox A's token against sandbox B's host fails.\
  \ It stays\n  sources:\n  - openapi/gmi-cloud-sandbox-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/gmi-cloud/refs/heads/main/authentication/gmi-cloud-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Company
- Artificial Intelligence
- Inference
- GPU Cloud
- LLM
- Model Routing
- Sandbox
- Infrastructure
---
