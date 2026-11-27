---
anonymous_access: false
api_key_in: []
api_specs:
- filename: google-cloud-vpc-operations-api-openapi.yml
  format: yaml
  label: Google Cloud VPC Operations API
  slug: google-cloud-vpc-operations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-cloud-vpc/openapi/google-cloud-vpc-operations-api-openapi.yml
- filename: google-cloud-vpc-organizations-api-openapi.yml
  format: yaml
  label: Google Cloud VPC Organizations API
  slug: google-cloud-vpc-organizations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-cloud-vpc/openapi/google-cloud-vpc-organizations-api-openapi.yml
- filename: google-cloud-vpc-projects-api-openapi.yml
  format: yaml
  label: Google Cloud VPC Projects API
  slug: google-cloud-vpc-projects-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-cloud-vpc/openapi/google-cloud-vpc-projects-api-openapi.yml
- filename: google-cloud-vpc-services-api-openapi.yml
  format: yaml
  label: Google Cloud VPC Services API
  slug: google-cloud-vpc-services-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-cloud-vpc/openapi/google-cloud-vpc-services-api-openapi.yml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Google Cloud VPC Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Google Cloud VPC secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Google Cloud VPC
provider_slug: google-cloud-vpc
scheme_count: 1
schemes:
- flows:
  - authorizationUrl: https://accounts.google.com/o/oauth2/auth
    flow: authorizationCode
    scopes: 2
    tokenUrl: https://oauth2.googleapis.com/token
  name: oauth2
  sources:
  - openapi/openapi.yml
  type: oauth2
slug: google-cloud-vpc-authentication
source_filename: google-cloud-vpc-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/openapi.yml\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: oauth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://accounts.google.com/o/oauth2/auth\n    tokenUrl: https://oauth2.googleapis.com/token\n    scopes: 2\n  sources:\n  - openapi/openapi.yml\n"
source_yaml_url: https://artifacts.apis.io/google-cloud-vpc/authentication/google-cloud-vpc-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Firewall
- Google Cloud
- Networking
- Virtual Networks
- VPC
---
