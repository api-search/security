---
api_key_in: []
api_specs:
- filename: productplan-bars-api-openapi.yml
  format: yaml
  label: ProductPlan Bars API
  slug: productplan-bars-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/productplan/refs/heads/main/openapi/productplan-bars-api-openapi.yml
- filename: productplan-discovery-api-openapi.yml
  format: yaml
  label: ProductPlan Discovery API
  slug: productplan-discovery-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/productplan/refs/heads/main/openapi/productplan-discovery-api-openapi.yml
- filename: productplan-launches-api-openapi.yml
  format: yaml
  label: ProductPlan Launches API
  slug: productplan-launches-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/productplan/refs/heads/main/openapi/productplan-launches-api-openapi.yml
- filename: productplan-roadmaps-api-openapi.yml
  format: yaml
  label: ProductPlan Roadmaps API
  slug: productplan-roadmaps-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/productplan/refs/heads/main/openapi/productplan-roadmaps-api-openapi.yml
- filename: productplan-status-api-openapi.yml
  format: yaml
  label: ProductPlan Status API
  slug: productplan-status-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/productplan/refs/heads/main/openapi/productplan-status-api-openapi.yml
- filename: productplan-strategy-api-openapi.yml
  format: yaml
  label: ProductPlan Strategy API
  slug: productplan-strategy-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/productplan/refs/heads/main/openapi/productplan-strategy-api-openapi.yml
- filename: productplan-teams-api-openapi.yml
  format: yaml
  label: ProductPlan Teams API
  slug: productplan-teams-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/productplan/refs/heads/main/openapi/productplan-teams-api-openapi.yml
- filename: productplan-users-api-openapi.yml
  format: yaml
  label: ProductPlan Users API
  slug: productplan-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/productplan/refs/heads/main/openapi/productplan-users-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Productplan Authentication
name_suffix: Authentication
oauth_flows: []
overview: ProductPlan secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: ProductPlan
provider_slug: productplan
scheme_count: 1
schemes:
- description: 'Personal Access Token (64-character hash). Generate in ProductPlan under Settings > Integrations. Include as: Authorization: Bearer <token>'
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/productplan-rest-api-openapi.yml
  type: http
slug: productplan-authentication
source_filename: productplan-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/productplan-rest-api-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: 'Personal Access Token (64-character hash). Generate in ProductPlan under Settings\n    > Integrations. Include as: Authorization: Bearer <token>'\n  sources:\n  - openapi/productplan-rest-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/productplan/refs/heads/main/authentication/productplan-authentication.yml
summary_line: http · 1 scheme
tags:
- Road Mapping
- Product Management
- OKR
- Roadmaps
- Features
- Product Strategy
- Launches
- Discovery
- Integrations
---
