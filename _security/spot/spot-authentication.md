---
api_key_in: []
api_specs:
- filename: spot-administration-api-openapi.yml
  format: yaml
  label: Spot Administration API
  slug: administration-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spot/refs/heads/main/openapi/spot-administration-api-openapi.yml
- filename: spot-elastigroup-api-openapi.yml
  format: yaml
  label: Spot Elastigroup API
  slug: elastigroup-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spot/refs/heads/main/openapi/spot-elastigroup-api-openapi.yml
- filename: spot-ocean-api-openapi.yml
  format: yaml
  label: Spot Ocean API
  slug: ocean-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spot/refs/heads/main/openapi/spot-ocean-api-openapi.yml
- filename: spot-eco-api-openapi.yml
  format: yaml
  label: Spot Eco API
  slug: eco-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spot/refs/heads/main/openapi/spot-eco-api-openapi.yml
- filename: spot-billing-engine-api-openapi.yml
  format: yaml
  label: Spot Billing Engine API
  slug: billing-engine-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spot/refs/heads/main/openapi/spot-billing-engine-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Spot Authentication
name_suffix: Authentication
oauth_flows: []
overview: Spot secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Spot
provider_slug: spot
scheme_count: 1
schemes:
- description: Spot API uses Bearer Token Authentication. Include your API token in the Authorization header.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/spot-administration-api-openapi.yml
  - openapi/spot-billing-engine-api-openapi.yml
  - openapi/spot-eco-api-openapi.yml
  - openapi/spot-elastigroup-api-openapi.yml
  - openapi/spot-ocean-api-openapi.yml
  type: http
slug: spot-authentication
source_filename: spot-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/spot-administration-api-openapi.yml, openapi/spot-billing-engine-api-openapi.yml,\n  openapi/spot-eco-api-openapi.yml, openapi/spot-elastigroup-api-openapi.yml, openapi/spot-ocean-api-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: Spot API uses Bearer Token Authentication. Include your API token in the Authorization\n    header.\n  sources:\n  - openapi/spot-administration-api-openapi.yml\n  - openapi/spot-billing-engine-api-openapi.yml\n  - openapi/spot-eco-api-openapi.yml\n  - openapi/spot-elastigroup-api-openapi.yml\n  - openapi/spot-ocean-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/spot/refs/heads/main/authentication/spot-authentication.yml
summary_line: http · 1 scheme
tags:
- Autoscaling
- Cloud Infrastructure
- Containers
- Cost Optimization
- FinOps
- Kubernetes
- Spot Instances
---
