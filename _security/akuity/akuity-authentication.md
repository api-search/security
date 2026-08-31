---
api_key_in: []
api_specs:
- filename: akuity-apikeyservice-api-openapi.yml
  format: yaml
  label: Akuity API Key Service API
  slug: akuity-apikeyservice-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/akuity/refs/heads/main/openapi/akuity-apikeyservice-api-openapi.yml
- filename: akuity-argocdservice-api-openapi.yml
  format: yaml
  label: Akuity Argo CD Service API
  slug: akuity-argocdservice-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/akuity/refs/heads/main/openapi/akuity-argocdservice-api-openapi.yml
- filename: akuity-authservice-api-openapi.yml
  format: yaml
  label: Akuity Auth Service API
  slug: akuity-authservice-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/akuity/refs/heads/main/openapi/akuity-authservice-api-openapi.yml
- filename: akuity-customroleservice-api-openapi.yml
  format: yaml
  label: Akuity Custom Role Service API
  slug: akuity-customroleservice-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/akuity/refs/heads/main/openapi/akuity-customroleservice-api-openapi.yml
- filename: akuity-extensionservice-api-openapi.yml
  format: yaml
  label: Akuity Extension Service API
  slug: akuity-extensionservice-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/akuity/refs/heads/main/openapi/akuity-extensionservice-api-openapi.yml
- filename: akuity-kargoservice-api-openapi.yml
  format: yaml
  label: Akuity Kargo Service API
  slug: akuity-kargoservice-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/akuity/refs/heads/main/openapi/akuity-kargoservice-api-openapi.yml
- filename: akuity-organizationservice-api-openapi.yml
  format: yaml
  label: Akuity Organization Service API
  slug: akuity-organizationservice-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/akuity/refs/heads/main/openapi/akuity-organizationservice-api-openapi.yml
- filename: akuity-systemservice-api-openapi.yml
  format: yaml
  label: Akuity System Service API
  slug: akuity-systemservice-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/akuity/refs/heads/main/openapi/akuity-systemservice-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Akuity Authentication
name_suffix: Authentication
oauth_flows: []
overview: Akuity secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Akuity
provider_slug: akuity
scheme_count: 1
schemes:
- description: 'HTTP Basic auth: username = AKUITY_API_KEY_ID, password = AKUITY_API_KEY_SECRET.'
  name: basicAuth
  scheme: basic
  sources:
  - openapi/akuity-apikey.json
  - openapi/akuity-argocd.json
  - openapi/akuity-auth.json
  - openapi/akuity-customrole.json
  - openapi/akuity-extension.json
  - openapi/akuity-kargo.json
  - openapi/akuity-organization.json
  - openapi/akuity-system.json
  type: http
slug: akuity-authentication
source_filename: akuity-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-06'\nmethod: derived\nsource: openapi/akuity-apikey.json, openapi/akuity-argocd.json, openapi/akuity-auth.json, openapi/akuity-customrole.json,\n  openapi/akuity-extension.json, openapi/akuity-kargo.json, openapi/akuity-organization.json,\n  openapi/akuity-system.json\nsummary:\n  types:\n  - http\nschemes:\n- name: basicAuth\n  type: http\n  scheme: basic\n  description: 'HTTP Basic auth: username = AKUITY_API_KEY_ID, password = AKUITY_API_KEY_SECRET.'\n  sources:\n  - openapi/akuity-apikey.json\n  - openapi/akuity-argocd.json\n  - openapi/akuity-auth.json\n  - openapi/akuity-customrole.json\n  - openapi/akuity-extension.json\n  - openapi/akuity-kargo.json\n  - openapi/akuity-organization.json\n  - openapi/akuity-system.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/akuity/refs/heads/main/authentication/akuity-authentication.yml
summary_line: http · 1 scheme
tags:
- GitOps
- Continuous Delivery
- Kubernetes
- Argo CD
- Kargo
- Platform Engineering
- DevOps
- Progressive Delivery
- Cloud-Native
- AIOps
- Developer Tools
---
