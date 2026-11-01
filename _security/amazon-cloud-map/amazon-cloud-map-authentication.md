---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: amazon-cloud-map-instances-api-openapi.yml
  format: yaml
  label: Amazon Cloud Map Instances API
  slug: amazon-cloud-map-instances-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-cloud-map/openapi/amazon-cloud-map-instances-api-openapi.yml
- filename: amazon-cloud-map-namespaces-api-openapi.yml
  format: yaml
  label: Amazon Cloud Map Namespaces API
  slug: amazon-cloud-map-namespaces-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-cloud-map/openapi/amazon-cloud-map-namespaces-api-openapi.yml
- filename: amazon-cloud-map-services-api-openapi.yml
  format: yaml
  label: Amazon Cloud Map Services API
  slug: amazon-cloud-map-services-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-cloud-map/openapi/amazon-cloud-map-services-api-openapi.yml
- filename: amazon-cloud-map-operations-api-openapi.yml
  format: yaml
  label: Amazon Cloud Map Cloud Map Operations API
  slug: amazon-cloud-map-operations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-cloud-map/openapi/amazon-cloud-map-operations-api-openapi.yml
- filename: amazon-cloud-map-service-attribute-api-openapi.yml
  format: yaml
  label: Amazon Cloud Map Cloud Map Service Attribute API
  slug: amazon-cloud-map-service-attribute-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-cloud-map/openapi/amazon-cloud-map-service-attribute-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Amazon Cloud Map Authentication
name_suffix: Authentication
oauth_flows: []
overview: Amazon Cloud Map secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Amazon Cloud Map
provider_slug: amazon-cloud-map
scheme_count: 1
schemes:
- description: AWS Signature Version 4
  in: header
  name: aws_signature
  parameter: Authorization
  sources:
  - openapi/amazon-cloud-map-openapi.yml
  type: apiKey
slug: amazon-cloud-map-authentication
source_filename: amazon-cloud-map-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/amazon-cloud-map-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: aws_signature\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: AWS Signature Version 4\n  sources:\n  - openapi/amazon-cloud-map-openapi.yml\n"
source_yaml_url: https://artifacts.apis.io/amazon-cloud-map/authentication/amazon-cloud-map-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Cloud Map
- Service Discovery
- Microservices
- DNS
---
