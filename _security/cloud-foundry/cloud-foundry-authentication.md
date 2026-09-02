---
api_key_in: []
api_specs:
- filename: cloud-foundry-apps-api-openapi.yml
  format: yaml
  label: Cloud Foundry Apps API
  slug: cloud-foundry-apps-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cloud-foundry/refs/heads/main/openapi/cloud-foundry-apps-api-openapi.yml
- filename: cloud-foundry-builds-api-openapi.yml
  format: yaml
  label: Cloud Foundry Builds API
  slug: cloud-foundry-builds-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cloud-foundry/refs/heads/main/openapi/cloud-foundry-builds-api-openapi.yml
- filename: cloud-foundry-cloud-foundry-cloud-controller-api-v3-api-openapi.yml
  format: yaml
  label: Cloud Foundry Cloud Foundry Cloud Controller API V3 API
  slug: cloud-foundry-cloud-foundry-cloud-controller-api-v3-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cloud-foundry/refs/heads/main/openapi/cloud-foundry-cloud-foundry-cloud-controller-api-v3-api-openapi.yml
- filename: cloud-foundry-deployments-api-openapi.yml
  format: yaml
  label: Cloud Foundry Deployments API
  slug: cloud-foundry-deployments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cloud-foundry/refs/heads/main/openapi/cloud-foundry-deployments-api-openapi.yml
- filename: cloud-foundry-jobs-api-openapi.yml
  format: yaml
  label: Cloud Foundry Jobs API
  slug: cloud-foundry-jobs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cloud-foundry/refs/heads/main/openapi/cloud-foundry-jobs-api-openapi.yml
- filename: cloud-foundry-organizations-api-openapi.yml
  format: yaml
  label: Cloud Foundry Organizations API
  slug: cloud-foundry-organizations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cloud-foundry/refs/heads/main/openapi/cloud-foundry-organizations-api-openapi.yml
- filename: cloud-foundry-service-instances-api-openapi.yml
  format: yaml
  label: Cloud Foundry Service Instances API
  slug: cloud-foundry-service-instances-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cloud-foundry/refs/heads/main/openapi/cloud-foundry-service-instances-api-openapi.yml
- filename: cloud-foundry-spaces-api-openapi.yml
  format: yaml
  label: Cloud Foundry Spaces API
  slug: cloud-foundry-spaces-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cloud-foundry/refs/heads/main/openapi/cloud-foundry-spaces-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Cloud Foundry Authentication
name_suffix: Authentication
oauth_flows: []
overview: Cloud Foundry secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Cloud Foundry
provider_slug: cloud-foundry
scheme_count: 1
schemes:
- bearerFormat: JWT
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/cloud-foundry-openapi.yml
  type: http
slug: cloud-foundry-authentication
source_filename: cloud-foundry-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/cloud-foundry-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  sources:\n  - openapi/cloud-foundry-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cloud-foundry/refs/heads/main/authentication/cloud-foundry-authentication.yml
summary_line: http · 1 scheme
tags:
- Cloud Foundry Foundation
- Containers
- Multi-Cloud
- Open-Source
- Platform-as-a-Service
- Platform
---
