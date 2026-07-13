---
api_key_in: []
api_specs:
- filename: drone-deploy-graphql-api-openapi.yml
  format: yaml
  label: DroneDeploy GraphQL API
  slug: drone-deploy-graphql-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/drone-deploy/refs/heads/main/openapi/drone-deploy-graphql-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Drone Deploy Authentication
name_suffix: Authentication
oauth_flows: []
overview: DroneDeploy secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: DroneDeploy
provider_slug: drone-deploy
scheme_count: 1
schemes:
- bearerFormat: API Key
  description: 'DroneDeploy API key sent as `Authorization: Bearer <api_key>`. Keys are issued by DroneDeploy Support (existing developers) or Sales (Developer Partner / Enterprise accounts). The same key is used for all GraphQL operations and is tied to the issuing user''s account.'
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/drone-deploy-graphql-api-openapi.yml
  type: http
slug: drone-deploy-authentication
source_filename: drone-deploy-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/drone-deploy-graphql-api-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: API Key\n  description: 'DroneDeploy API key sent as `Authorization: Bearer <api_key>`. Keys are issued\n    by DroneDeploy Support (existing developers) or Sales (Developer Partner / Enterprise accounts).\n    The same key is used for all GraphQL operations and is tied to the issuing user''s account.'\n  sources:\n  - openapi/drone-deploy-graphql-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/drone-deploy/refs/heads/main/authentication/drone-deploy-authentication.yml
summary_line: http · 1 scheme
tags:
- Drones
- Reality Capture
- Mapping
- Photogrammetry
- 3D Models
- Orthomosaic
- LiDAR
- Construction
- Agriculture
- AI
- Aerial
- Robotics
---
