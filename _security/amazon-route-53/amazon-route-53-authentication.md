---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: amazon-route-53-health-checks-api-openapi.yml
  format: yaml
  label: Amazon Route 53 Health Checks API
  slug: amazon-route-53-health-checks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-route-53/openapi/amazon-route-53-health-checks-api-openapi.yml
- filename: amazon-route-53-hosted-zones-api-openapi.yml
  format: yaml
  label: Amazon Route 53 Hosted Zones API
  slug: amazon-route-53-hosted-zones-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-route-53/openapi/amazon-route-53-hosted-zones-api-openapi.yml
- filename: amazon-route-53-resource-record-sets-api-openapi.yml
  format: yaml
  label: Amazon Route 53 Resource Record Sets API
  slug: amazon-route-53-resource-record-sets-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-route-53/openapi/amazon-route-53-resource-record-sets-api-openapi.yml
- filename: amazon-route-53-cidrcollection-api-openapi.yml
  format: yaml
  label: Amazon Route 53 Route 53 Cidrcollection API
  slug: amazon-route-53-cidrcollection-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-route-53/openapi/amazon-route-53-cidrcollection-api-openapi.yml
- filename: amazon-route-53-delegationset-api-openapi.yml
  format: yaml
  label: Amazon Route 53 Route 53 Delegationset API
  slug: amazon-route-53-delegationset-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-route-53/openapi/amazon-route-53-delegationset-api-openapi.yml
- filename: amazon-route-53-operations-api-openapi.yml
  format: yaml
  label: Amazon Route 53 Route 53 Operations API
  slug: amazon-route-53-operations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-route-53/openapi/amazon-route-53-operations-api-openapi.yml
- filename: amazon-route-53-queryloggingconfig-api-openapi.yml
  format: yaml
  label: Amazon Route 53 Route 53 Queryloggingconfig API
  slug: amazon-route-53-queryloggingconfig-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-route-53/openapi/amazon-route-53-queryloggingconfig-api-openapi.yml
- filename: amazon-route-53-tags-api-openapi.yml
  format: yaml
  label: Amazon Route 53 Route 53 Tags API
  slug: amazon-route-53-tags-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-route-53/openapi/amazon-route-53-tags-api-openapi.yml
- filename: amazon-route-53-trafficpolicy-api-openapi.yml
  format: yaml
  label: Amazon Route 53 Route 53 Trafficpolicy API
  slug: amazon-route-53-trafficpolicy-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-route-53/openapi/amazon-route-53-trafficpolicy-api-openapi.yml
- filename: amazon-route-53-trafficpolicyinstance-api-openapi.yml
  format: yaml
  label: Amazon Route 53 Route 53 Trafficpolicyinstance API
  slug: amazon-route-53-trafficpolicyinstance-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-route-53/openapi/amazon-route-53-trafficpolicyinstance-api-openapi.yml
- filename: amazon-route-53-trafficpolicyinstances-api-openapi.yml
  format: yaml
  label: Amazon Route 53 Route 53 Trafficpolicyinstances API
  slug: amazon-route-53-trafficpolicyinstances-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-route-53/openapi/amazon-route-53-trafficpolicyinstances-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Amazon Route 53 Authentication
name_suffix: Authentication
oauth_flows: []
overview: Amazon Route 53 secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Amazon Route 53
provider_slug: amazon-route-53
scheme_count: 1
schemes:
- description: AWS Signature Version 4 authentication
  in: header
  name: aws_sig_v4
  parameter: Authorization
  sources:
  - openapi/amazon-route-53-openapi.yml
  type: apiKey
slug: amazon-route-53-authentication
source_filename: amazon-route-53-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/amazon-route-53-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: aws_sig_v4\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: AWS Signature Version 4 authentication\n  sources:\n  - openapi/amazon-route-53-openapi.yml\n"
source_yaml_url: https://artifacts.apis.io/amazon-route-53/authentication/amazon-route-53-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- DNS
- Domain Registration
- Health Checks
- Routing
---
