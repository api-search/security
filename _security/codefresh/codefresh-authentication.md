---
api_key_in:
- header
api_specs:
- filename: codefresh-access-control-api-openapi.yml
  format: yaml
  label: Codefresh Access Control API
  slug: codefresh-access-control-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/codefresh/refs/heads/main/openapi/codefresh-access-control-api-openapi.yml
- filename: codefresh-accounts-api-openapi.yml
  format: yaml
  label: Codefresh Accounts API
  slug: codefresh-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/codefresh/refs/heads/main/openapi/codefresh-accounts-api-openapi.yml
- filename: codefresh-admin-api-openapi.yml
  format: yaml
  label: Codefresh Admin API
  slug: codefresh-admin-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/codefresh/refs/heads/main/openapi/codefresh-admin-api-openapi.yml
- filename: codefresh-annotations-api-openapi.yml
  format: yaml
  label: Codefresh Annotations API
  slug: codefresh-annotations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/codefresh/refs/heads/main/openapi/codefresh-annotations-api-openapi.yml
- filename: codefresh-audit-api-openapi.yml
  format: yaml
  label: Codefresh Audit API
  slug: codefresh-audit-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/codefresh/refs/heads/main/openapi/codefresh-audit-api-openapi.yml
- filename: codefresh-auth-api-openapi.yml
  format: yaml
  label: Codefresh Auth API
  slug: codefresh-auth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/codefresh/refs/heads/main/openapi/codefresh-auth-api-openapi.yml
- filename: codefresh-builds-api-openapi.yml
  format: yaml
  label: Codefresh Builds API
  slug: codefresh-builds-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/codefresh/refs/heads/main/openapi/codefresh-builds-api-openapi.yml
- filename: codefresh-clusters-api-openapi.yml
  format: yaml
  label: Codefresh Clusters API
  slug: codefresh-clusters-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/codefresh/refs/heads/main/openapi/codefresh-clusters-api-openapi.yml
- filename: codefresh-contexts-api-openapi.yml
  format: yaml
  label: Codefresh Contexts API
  slug: codefresh-contexts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/codefresh/refs/heads/main/openapi/codefresh-contexts-api-openapi.yml
- filename: codefresh-environments-api-openapi.yml
  format: yaml
  label: Codefresh Environments API
  slug: codefresh-environments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/codefresh/refs/heads/main/openapi/codefresh-environments-api-openapi.yml
- filename: codefresh-features-api-openapi.yml
  format: yaml
  label: Codefresh Features API
  slug: codefresh-features-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/codefresh/refs/heads/main/openapi/codefresh-features-api-openapi.yml
- filename: codefresh-helm-api-openapi.yml
  format: yaml
  label: Codefresh Helm API
  slug: codefresh-helm-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/codefresh/refs/heads/main/openapi/codefresh-helm-api-openapi.yml
- filename: codefresh-workflows-api-openapi.yml
  format: yaml
  label: Codefresh Workflows API
  slug: codefresh-workflows-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/codefresh/refs/heads/main/openapi/codefresh-workflows-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Codefresh Authentication
name_suffix: Authentication
oauth_flows: []
overview: Codefresh secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Codefresh
provider_slug: codefresh
scheme_count: 1
schemes:
- description: Codefresh API key. Send raw token as Authorization header value.
  in: header
  name: ApiKeyAuth
  parameter: Authorization
  sources:
  - openapi/codefresh-openapi.yml
  type: apiKey
slug: codefresh-authentication
source_filename: codefresh-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/codefresh-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: Codefresh API key. Send raw token as Authorization header value.\n  sources:\n  - openapi/codefresh-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/codefresh/refs/heads/main/authentication/codefresh-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- CI/CD
- Continuous Delivery
- GitOps
- Argo
- Kubernetes
- DevOps
- Pipelines
---
