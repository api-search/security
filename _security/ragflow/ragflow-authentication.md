---
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
method: searched
name: Ragflow Authentication
name_suffix: Authentication
oauth_flows: []
overview: RAGFlow declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: RAGFlow
provider_slug: ragflow
scheme_count: 1
schemes:
- applies_to: all 95 documented operations except GET /api/v1/system/healthz
  description: A RAGFlow API key issued per tenant from the RAGFlow UI (avatar in the top-right corner -> API). The reference presents this header on every request example in the document.
  expiry: not documented
  format: 'Authorization: Bearer <YOUR_API_KEY>'
  id: bearerApiKey
  in: header
  name: Authorization
  rotation: Keys are created and revoked from the same UI page. No rotation policy, expiry or grace period is documented, and there is no API to mint or revoke a key.
  scheme: bearer
  scope_model: none
  scopes: []
  type: http
slug: ragflow-authentication
source_filename: ragflow-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-27'\nmethod: searched\nsource: https://ragflow.io/docs/acquire_ragflow_api_key + https://ragflow.io/docs/http_api_reference\ndocs: https://ragflow.io/docs/acquire_ragflow_api_key\napi: ragflow-http-api\nsummary: >-\n  A single authentication scheme covers the entire RAGFlow surface: a tenant-scoped API key presented as\n  an HTTP bearer token. There is no OAuth 2.0, no OpenID Connect, no mutual TLS, no signed requests and\n  no scope system. The same key authenticates the HTTP API, the Python SDK and the MCP server.\nschemes:\n- id: bearerApiKey\n  type: http\n  scheme: bearer\n  in: header\n  name: Authorization\n  format: 'Authorization: Bearer <YOUR_API_KEY>'\n  applies_to: all 95 documented operations except GET /api/v1/system/healthz\n  description: >-\n    A RAGFlow API key issued per tenant from the RAGFlow UI (avatar in the top-right corner -> API).\n    The reference presents this header on every request example in the document.\n  rotation: >-\n\
  \    Keys are created and revoked from the same UI page. No rotation policy, expiry or grace period is\n    documented, and there is no API to mint or revoke a key.\n  expiry: not documented\n  scopes: []\n  scope_model: none\nunauthenticated_operations:\n- operation: GET /api/v1/system/healthz\n  note: >-\n    Verified live on 2026-08-27 — https://cloud.ragflow.io/api/v1/system/healthz returns HTTP 200 with\n    {\"db\":\"ok\",\"doc_engine\":\"ok\",\"redis\":\"ok\",\"status\":\"ok\",\"storage\":\"ok\"} without any Authorization\n    header.\noauth2: false\nopenid_connect: false\nmutual_tls: false\nwebhook_signing: not applicable — RAGFlow publishes no webhooks\nfailure_behaviour:\n  missing_or_invalid_key:\n    http_status: 401\n    body: '{\"code\":401,\"data\":null,\"message\":\"<Unauthorized ''401: Unauthorized'' >\"}'\n    observed_at: https://cloud.ragflow.io/api/v1/datasets?page=1&page_size=1\n    observed_on: '2026-08-27'\n    www_authenticate_header: false\n  handler_level:\n\
  \    code: 109\n    message: no authorization\n  insufficient_permission:\n    code: 108\n    message: tenant lacks permission for the named datasets\n  not_owner:\n    code: 103\n    message: Only owner of canvas authorized for this operation.\navailability:\n  self_hosted: >-\n    Any RAGFlow deployment can issue API keys — this is the full-capability path, and the reason the\n    API surface is documented against http://{address}/api/v1.\n  cloud:\n    free: false\n    free_note: >-\n      The RAGFlow Cloud pricing page states \"API key not available\" on the Free plan. A Cloud evaluator\n      cannot call the API without paying, which is the single largest onboarding friction on this\n      provider.\n    starter: true\n    pro: true\n    enterprise: true\nmulti_tenancy:\n  model: >-\n    A key is bound to one tenant. The MCP server's self-host mode holds one key and therefore sees one\n    tenant's datasets; host mode requires each client to present its own key so each sees its own.\n\
  gaps:\n- No scopes — a key that can read a dataset can also delete every dataset, chat assistant and agent in\n  the tenant. There is no read-only key.\n- No key expiry, no documented rotation policy, and no programmatic key management.\n- No WWW-Authenticate header on 401, so a client cannot discover the scheme from a challenge.\n- No OAuth or OIDC, so RAGFlow cannot participate in a delegated-consent agent flow.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ragflow/refs/heads/main/authentication/ragflow-authentication.yml
summary_line: 1 scheme
tags:
- Company
- Artificial Intelligence
- Retrieval Augmented Generation
- Search
- Vector Database
- Document Processing
- Knowledge Management
- Agents
- Open Source
- LLM
- Model Context Protocol
---
