---
api_key_in: []
api_specs:
- filename: kserve-openapi.yml
  format: yaml
  label: KServe Inference API
  slug: inference-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kserve/refs/heads/main/openapi/kserve-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Kserve Authentication
name_suffix: Authentication
oauth_flows: []
overview: KServe secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: KServe
provider_slug: kserve
scheme_count: 1
schemes:
- description: 'KServe itself does not mandate an auth scheme; in production the

    InferenceService is typically fronted by an ingress/gateway that

    enforces auth (for example, Istio with OIDC/JWT, Knative serving

    with Kubernetes auth, or an API gateway). Bearer tokens are the

    most common production pattern.'
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/kserve-openapi.yml
  type: http
slug: kserve-authentication
source_filename: kserve-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/kserve-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  description: |-\n    KServe itself does not mandate an auth scheme; in production the\n    InferenceService is typically fronted by an ingress/gateway that\n    enforces auth (for example, Istio with OIDC/JWT, Knative serving\n    with Kubernetes auth, or an API gateway). Bearer tokens are the\n    most common production pattern.\n  sources:\n  - openapi/kserve-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/kserve/refs/heads/main/authentication/kserve-authentication.yml
summary_line: http · 1 scheme
tags:
- Inference
- Kubernetes
- Machine Learning
- MLOps
- Model Serving
---
