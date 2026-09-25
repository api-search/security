---
anonymous_access: false
api_key_in: []
api_specs:
- filename: densify-analysis-webhook-api-openapi.yml
  format: yaml
  label: Densify Analysis Webhook API
  slug: densify-analysis-webhook-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/densify/refs/heads/main/openapi/densify-analysis-webhook-api-openapi.yml
- filename: densify-authentication-api-openapi.yml
  format: yaml
  label: Densify Authentication API
  slug: densify-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/densify/refs/heads/main/openapi/densify-authentication-api-openapi.yml
- filename: densify-aws-analysis-api-openapi.yml
  format: yaml
  label: Densify AWS Analysis API
  slug: densify-aws-analysis-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/densify/refs/heads/main/openapi/densify-aws-analysis-api-openapi.yml
- filename: densify-aws-analyze-api-openapi.yml
  format: yaml
  label: Densify AWS Analyze API
  slug: densify-aws-analyze-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/densify/refs/heads/main/openapi/densify-aws-analyze-api-openapi.yml
- filename: densify-azure-analysis-api-openapi.yml
  format: yaml
  label: Densify Azure Analysis API
  slug: densify-azure-analysis-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/densify/refs/heads/main/openapi/densify-azure-analysis-api-openapi.yml
- filename: densify-cloud-analysis-api-openapi.yml
  format: yaml
  label: Densify Cloud Analysis API
  slug: densify-cloud-analysis-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/densify/refs/heads/main/openapi/densify-cloud-analysis-api-openapi.yml
- filename: densify-gcp-analysis-api-openapi.yml
  format: yaml
  label: Densify GCP Analysis API
  slug: densify-gcp-analysis-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/densify/refs/heads/main/openapi/densify-gcp-analysis-api-openapi.yml
- filename: densify-kubernetes-api-openapi.yml
  format: yaml
  label: Densify Kubernetes API
  slug: densify-kubernetes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/densify/refs/heads/main/openapi/densify-kubernetes-api-openapi.yml
- filename: densify-kubernetes-cluster-results-api-openapi.yml
  format: yaml
  label: Densify Kubernetes Cluster Results API
  slug: densify-kubernetes-cluster-results-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/densify/refs/heads/main/openapi/densify-kubernetes-cluster-results-api-openapi.yml
- filename: densify-kubernetes-clusters-api-openapi.yml
  format: yaml
  label: Densify Kubernetes Clusters API
  slug: densify-kubernetes-clusters-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/densify/refs/heads/main/openapi/densify-kubernetes-clusters-api-openapi.yml
- filename: densify-recommendations-api-openapi.yml
  format: yaml
  label: Densify Recommendations API
  slug: densify-recommendations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/densify/refs/heads/main/openapi/densify-recommendations-api-openapi.yml
- filename: densify-subscriptions-api-openapi.yml
  format: yaml
  label: Densify Subscriptions API
  slug: densify-subscriptions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/densify/refs/heads/main/openapi/densify-subscriptions-api-openapi.yml
- filename: densify-subscriptions-properties-api-openapi.yml
  format: yaml
  label: Densify Subscriptions Properties API
  slug: densify-subscriptions-properties-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/densify/refs/heads/main/openapi/densify-subscriptions-properties-api-openapi.yml
- filename: densify-subscriptions-suppressions-api-openapi.yml
  format: yaml
  label: Densify Subscriptions Suppressions API
  slug: densify-subscriptions-suppressions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/densify/refs/heads/main/openapi/densify-subscriptions-suppressions-api-openapi.yml
- filename: densify-subscriptions-tags-api-openapi.yml
  format: yaml
  label: Densify Subscriptions Tags API
  slug: densify-subscriptions-tags-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/densify/refs/heads/main/openapi/densify-subscriptions-tags-api-openapi.yml
- filename: densify-system-api-openapi.yml
  format: yaml
  label: Densify System API
  slug: densify-system-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/densify/refs/heads/main/openapi/densify-system-api-openapi.yml
- filename: densify-systems-api-openapi.yml
  format: yaml
  label: Densify Systems API
  slug: densify-systems-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/densify/refs/heads/main/openapi/densify-systems-api-openapi.yml
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Densify Authentication
name_suffix: Authentication
oauth_flows: []
overview: Densify secures its APIs with http and oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Densify
provider_slug: densify
scheme_count: 1
schemes:
- bearerFormat: JWT
  description: 'Apply to **other** API endpoints after obtaining a token from `/authorize`.

    Example: `Authorization: Bearer <apiToken>`'
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/densify-authorize-openapi.yaml
  - openapi/densify-kubernetes-kubernetes-clusters-openapi.yaml
  - openapi/densify-kubernetes-kubernetes-clusters-results-openapi.yaml
  - openapi/densify-systems-openapi.yaml
  type: http
slug: densify-authentication
source_filename: densify-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-06'\nmethod: searched\nsource: >-\n  https://docs.kubex.ai/docs-api/WebHelp_Densify_API_Cloud/Content/API_Guide/Authorize/authorize-user\n  and https://docs.kubex.ai/docs-api/WebHelp_Densify_API_Cloud/Content/API_Guide/MCP,\n  cross-checked against openapi/densify-authorize-openapi.yaml\ndocs: https://docs.kubex.ai/docs-api/WebHelp_Densify_API_Cloud/Content/API_Guide/Authorize\nprovider: Densify\nproviderId: densify\nsummary:\n  types:\n  - http\n  - oauth2\n  models: 2\n  note: >-\n    The REST API uses a username/password exchange for a short-lived JWT bearer token. The\n    MCP surface uses a different model entirely — OAuth 2.1 with dynamic client registration —\n    so an agent integrating both needs two credential paths.\nmodels:\n- id: rest-jwt\n  surface: REST API (openapi/)\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  token_endpoint: POST /authorize\n  token_endpoint_operationId: authorize-user\n  credential: >-\n    JSON body with `userName`\
  \ and `pwd` for an ACTIVE Kubex user. Only tokens issued to\n    API-ENABLED users can be used to make authorized API calls — an active but non-API-enabled\n    user receives a token that every downstream call rejects.\n  token_lifetime_seconds: 3600\n  token_lifetime_note: >-\n    60 minutes. Raised from 5 minutes in the 3.0.0 release (2025-04-23) so longer-running\n    pipeline operations no longer need to re-authorize mid-run.\n  response_fields:\n  - apiToken\n  - expires\n  - status\n  header: 'Authorization: Bearer <apiToken>'\n  unauthenticated_operations:\n  - ping\n  failure_codes:\n  - status: 400\n    meaning: null/invalid payload; empty or invalid userName/pwd\n  - status: 401\n    meaning: user does not exist, incorrect password, or account locked\n  - status: 403\n    meaning: trial or subscription expired\n  - status: 429\n    meaning: too many requests — progressive delay applied to repeated authorization failures\n  sources:\n  - openapi/densify-authorize-openapi.yaml\n\
  - id: mcp-oauth\n  surface: Kubex MCP server (mcp/)\n  type: oauth2\n  profile: OAuth 2.1\n  dynamic_client_registration: true\n  endpoint_template: https://{company}-mcp.kubex.ai/\n  session: >-\n    Authorization is temporary and must be refreshed daily; clients that do not re-prompt on\n    expiry surface connection errors or incomplete responses.\n  scopes:\n    published: false\n    note: >-\n      No scope or permission reference is published. No /.well-known/oauth-authorization-server\n      or /.well-known/oauth-protected-resource document is served on any Densify or Kubex host\n      (all probed 404 on 2026-09-06), so the authorization-server metadata cannot be read\n      anonymously and no scopes/ artifact is emitted.\n  sources:\n  - https://docs.kubex.ai/docs-api/WebHelp_Densify_API_Cloud/Content/API_Guide/MCP\nsso:\n  available: true\n  tier: Enterprise K8s and GPU Optimization plan only\n  source: https://kubex.ai/kubex-pricing.md\n  note: >-\n    Single sign-on with the\
  \ customer's identity provider is an Enterprise-plan feature. The\n    docs also cover external user authentication against Azure AD, Google OpenID and Okta for\n    console login (not for the API).\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: |-\n    Apply to **other** API endpoints after obtaining a token from `/authorize`.\n    Example: `Authorization: Bearer <apiToken>`\n  sources:\n  - openapi/densify-authorize-openapi.yaml\n  - openapi/densify-kubernetes-kubernetes-clusters-openapi.yaml\n  - openapi/densify-kubernetes-kubernetes-clusters-results-openapi.yaml\n  - openapi/densify-systems-openapi.yaml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/densify/refs/heads/main/authentication/densify-authentication.yml
summary_line: http/oauth2 · 1 scheme
tags:
- Cloud Cost
- Container Optimization
- FinOps
- Kubernetes
- Machine Learning
- Recommendations
- Rightsizing
- A2A
---
