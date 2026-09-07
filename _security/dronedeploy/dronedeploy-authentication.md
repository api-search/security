---
anonymous_access: false
api_key_in: []
api_specs:
- filename: dronedeploy.postman_collection.json
  format: json
  label: DroneDeploy Projects and Plans API
  slug: dronedeploy-projects-and-plans-api
  spec_type: Postman
  url: https://raw.githubusercontent.com/api-evangelist/dronedeploy/refs/heads/main/collections/dronedeploy.postman_collection.json
- filename: dronedeploy.postman_collection.json
  format: json
  label: DroneDeploy Maps and Exports API
  slug: dronedeploy-maps-and-exports-api
  spec_type: Postman
  url: https://raw.githubusercontent.com/api-evangelist/dronedeploy/refs/heads/main/collections/dronedeploy.postman_collection.json
- filename: dronedeploy.postman_collection.json
  format: json
  label: DroneDeploy Annotations and Issues API
  slug: dronedeploy-annotations-and-issues-api
  spec_type: Postman
  url: https://raw.githubusercontent.com/api-evangelist/dronedeploy/refs/heads/main/collections/dronedeploy.postman_collection.json
- filename: dronedeploy.postman_collection.json
  format: json
  label: DroneDeploy Uploads and Images API
  slug: dronedeploy-uploads-and-images-api
  spec_type: Postman
  url: https://raw.githubusercontent.com/api-evangelist/dronedeploy/refs/heads/main/collections/dronedeploy.postman_collection.json
- filename: dronedeploy.postman_collection.json
  format: json
  label: DroneDeploy Users and Organizations API
  slug: dronedeploy-users-and-organizations-api
  spec_type: Postman
  url: https://raw.githubusercontent.com/api-evangelist/dronedeploy/refs/heads/main/collections/dronedeploy.postman_collection.json
- filename: dronedeploy.postman_collection.json
  format: json
  label: DroneDeploy Reports API
  slug: dronedeploy-reports-api
  spec_type: Postman
  url: https://raw.githubusercontent.com/api-evangelist/dronedeploy/refs/heads/main/collections/dronedeploy.postman_collection.json
- filename: dronedeploy.postman_collection.json
  format: json
  label: DroneDeploy Webhooks API
  slug: dronedeploy-webhooks-api
  spec_type: Postman
  url: https://raw.githubusercontent.com/api-evangelist/dronedeploy/refs/heads/main/collections/dronedeploy.postman_collection.json
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Dronedeploy Authentication
name_suffix: Authentication
oauth_flows: []
overview: DroneDeploy secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: DroneDeploy
provider_slug: dronedeploy
scheme_count: 1
schemes:
- bearerFormat: API Key
  description: 'DroneDeploy API key sent as `Authorization: Bearer <api_key>`. Keys are issued by DroneDeploy Support (existing developers) or Sales (Developer Partner / Enterprise accounts). The same key is used for all GraphQL operations and is tied to the issuing user''s account.'
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/drone-deploy-graphql-api-openapi.yml
  type: http
slug: dronedeploy-authentication
source_filename: dronedeploy-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/drone-deploy-graphql-api-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: API Key\n  description: 'DroneDeploy API key sent as `Authorization: Bearer <api_key>`. Keys are issued\n    by DroneDeploy Support (existing developers) or Sales (Developer Partner / Enterprise accounts).\n    The same key is used for all GraphQL operations and is tied to the issuing user''s account.'\n  sources:\n  - openapi/drone-deploy-graphql-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/dronedeploy/refs/heads/main/authentication/dronedeploy-authentication.yml
summary_line: http · 1 scheme
tags:
- Drone Mapping
- Reality Capture
- Aerial Analytics
- Geospatial
- GraphQL
- Photogrammetry
---
