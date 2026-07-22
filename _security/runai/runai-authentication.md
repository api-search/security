---
api_key_in: []
api_specs:
- filename: runai-openapi-original.json
  format: json
  label: NVIDIA Run:ai Control Plane REST API
  slug: nvidia-runai-control-plane-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/runai/refs/heads/main/openapi/runai-openapi-original.json
auth_types:
- http
description: ''
kind: authentication
layout: security
method: searched
name: Runai Authentication
name_suffix: Authentication
oauth_flows: []
overview: NVIDIA Run:ai secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: NVIDIA Run:ai
provider_slug: runai
scheme_count: 1
schemes:
- bearerFormat: JWT
  description: Bearer authentication
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/runai-openapi-original.json
  type: http
slug: runai-authentication
source_filename: runai-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: openapi/runai-openapi-original.json\ndocs: https://run-ai-docs.nvidia.com/api/getting-started/how-to-authenticate-to-the-api.md\nsummary:\n  types:\n  - http\n  model: bearer-jwt via client-credentials access key\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: Bearer authentication\n  sources:\n  - openapi/runai-openapi-original.json\ntoken_exchange:\n  endpoint: POST https://<COMPANY-URL>/api/v1/token\n  grant_type: client_credentials\n  request: '{\"grantType\":\"client_credentials\",\"clientId\":\"<CLIENT ID>\",\"clientSecret\":\"<CLIENT SECRET>\"}'\n  response: '{\"accessToken\":\"<TOKEN>\"}'\n  usage: Pass accessToken as a Bearer token in the Authorization header.\n  company_url:\n    saas: <tenant-name>.run.ai\n    self_hosted: the Run:ai user interface URL\ncredentials:\n  access_key: clientId + clientSecret, issued to a user or a service account\n  user_access_keys:\
  \ https://run-ai-docs.nvidia.com/saas/settings/user-settings/user-access-keys.md\n  service_accounts: https://run-ai-docs.nvidia.com/saas/infrastructure-setup/authentication/service-accounts.md\n  authorization: Access rules bind roles to subjects (see docs access rules / roles).\nsso:\n  user_login: SAML and OpenID Connect (OIDC) supported for UI/user login (not the API token flow).\n  docs: https://run-ai-docs.nvidia.com/saas/infrastructure-setup/authentication/sso.md\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/runai/refs/heads/main/authentication/runai-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Artificial Intelligence
- GPU
- Machine Learning
- Kubernetes
- Orchestration
- MLOps
- Compute
- Scheduling
- Infrastructure
---
