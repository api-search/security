---
anonymous_access: false
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Kinference Authentication
name_suffix: Authentication
oauth_flows: []
overview: Kinference declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Kinference
provider_slug: kinference-ai
scheme_count: 2
schemes:
- applies_to: Kinference Picker gRPC API
  description: 'Optional [token_review] section: "Validate Kubernetes bearer tokens for callers that cannot reach the apiserver themselves. Needs create on tokenreviews in authentication.k8s.io." Serves TokenReview on the gRPC listener; disabled by default. Authenticated results cached 60s, denied results 10s by default.'
  name: kubernetes-token-review
  scheme: bearer
  type: http
- description: The CRD API (kinference.buoyant.io/v1alpha1) is served by the customer's own Kubernetes API server, so access follows cluster RBAC.
  name: kubernetes-rbac
  type: kubernetes
slug: kinference-ai-authentication
source_filename: kinference-ai-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-05'\nmethod: searched\nsource: https://kinference.ai/docs/reference/config/\ndocs: https://kinference.ai/docs/reference/config/\nschemes:\n- name: kubernetes-token-review\n  type: http\n  scheme: bearer\n  description: 'Optional [token_review] section: \"Validate Kubernetes bearer tokens for callers that cannot reach the apiserver themselves. Needs create on tokenreviews in authentication.k8s.io.\" Serves TokenReview on the gRPC listener; disabled by default. Authenticated results cached 60s, denied results 10s by default.'\n  applies_to: Kinference Picker gRPC API\n- name: kubernetes-rbac\n  type: kubernetes\n  description: The CRD API (kinference.buoyant.io/v1alpha1) is served by the customer's own Kubernetes API server, so access follows cluster RBAC.\nnote: Self-hosted; no provider-issued API keys. Upstream InferenceProvider credentials are configured per backend (a BackendUnauthorized state is documented on the InferenceProvider CRD page).\n"
source_yaml_url: https://artifacts.apis.io/kinference-ai/authentication/kinference-ai-authentication.yml
summary_line: 2 schemes
tags:
- Company
- Inference
- Kubernetes
- vLLM
- LLM Gateway
- Rate Limiting
- Load Balancing
- Open Source
- Platform Engineering
---
