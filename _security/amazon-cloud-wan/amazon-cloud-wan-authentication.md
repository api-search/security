---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: amazon-cloud-wan-core-networks-api-openapi.yml
  format: yaml
  label: Amazon Cloud WAN Core Networks API
  slug: amazon-cloud-wan-core-networks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-cloud-wan/openapi/amazon-cloud-wan-core-networks-api-openapi.yml
- filename: amazon-cloud-wan-connect-peer-associations-api-openapi.yml
  format: yaml
  label: Amazon Cloud WAN Cloud Wan Connect Peer Associations API
  slug: amazon-cloud-wan-connect-peer-associations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-cloud-wan/openapi/amazon-cloud-wan-connect-peer-associations-api-openapi.yml
- filename: amazon-cloud-wan-connect-peers-api-openapi.yml
  format: yaml
  label: Amazon Cloud WAN Cloud Wan Connect Peers API
  slug: amazon-cloud-wan-connect-peers-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-cloud-wan/openapi/amazon-cloud-wan-connect-peers-api-openapi.yml
- filename: amazon-cloud-wan-connections-api-openapi.yml
  format: yaml
  label: Amazon Cloud WAN Cloud Wan Connections API
  slug: amazon-cloud-wan-connections-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-cloud-wan/openapi/amazon-cloud-wan-connections-api-openapi.yml
- filename: amazon-cloud-wan-customer-gateway-associations-api-openapi.yml
  format: yaml
  label: Amazon Cloud WAN Cloud Wan Customer Gateway Associations API
  slug: amazon-cloud-wan-customer-gateway-associations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-cloud-wan/openapi/amazon-cloud-wan-customer-gateway-associations-api-openapi.yml
- filename: amazon-cloud-wan-devices-api-openapi.yml
  format: yaml
  label: Amazon Cloud WAN Cloud Wan Devices API
  slug: amazon-cloud-wan-devices-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-cloud-wan/openapi/amazon-cloud-wan-devices-api-openapi.yml
- filename: amazon-cloud-wan-direct-connect-gateway-attachments-api-openapi.yml
  format: yaml
  label: Amazon Cloud WAN Cloud Wan Direct Connect Gateway Attachments API
  slug: amazon-cloud-wan-direct-connect-gateway-attachments-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-cloud-wan/openapi/amazon-cloud-wan-direct-connect-gateway-attachments-api-openapi.yml
- filename: amazon-cloud-wan-global-networks-api-openapi.yml
  format: yaml
  label: Amazon Cloud WAN Cloud Wan Global Networks API
  slug: amazon-cloud-wan-global-networks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-cloud-wan/openapi/amazon-cloud-wan-global-networks-api-openapi.yml
- filename: amazon-cloud-wan-link-associations-api-openapi.yml
  format: yaml
  label: Amazon Cloud WAN Cloud Wan Link Associations API
  slug: amazon-cloud-wan-link-associations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-cloud-wan/openapi/amazon-cloud-wan-link-associations-api-openapi.yml
- filename: amazon-cloud-wan-links-api-openapi.yml
  format: yaml
  label: Amazon Cloud WAN Cloud Wan Links API
  slug: amazon-cloud-wan-links-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-cloud-wan/openapi/amazon-cloud-wan-links-api-openapi.yml
- filename: amazon-cloud-wan-operations-api-openapi.yml
  format: yaml
  label: Amazon Cloud WAN Cloud Wan Operations API
  slug: amazon-cloud-wan-operations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-cloud-wan/openapi/amazon-cloud-wan-operations-api-openapi.yml
- filename: amazon-cloud-wan-resource-policy-api-openapi.yml
  format: yaml
  label: Amazon Cloud WAN Cloud Wan Resource Policy API
  slug: amazon-cloud-wan-resource-policy-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-cloud-wan/openapi/amazon-cloud-wan-resource-policy-api-openapi.yml
- filename: amazon-cloud-wan-sites-api-openapi.yml
  format: yaml
  label: Amazon Cloud WAN Cloud Wan Sites API
  slug: amazon-cloud-wan-sites-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-cloud-wan/openapi/amazon-cloud-wan-sites-api-openapi.yml
- filename: amazon-cloud-wan-tags-api-openapi.yml
  format: yaml
  label: Amazon Cloud WAN Cloud Wan Tags API
  slug: amazon-cloud-wan-tags-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-cloud-wan/openapi/amazon-cloud-wan-tags-api-openapi.yml
- filename: amazon-cloud-wan-transit-gateway-connect-peer-associations-api-openapi.yml
  format: yaml
  label: Amazon Cloud WAN Cloud Wan Transit Gateway Connect Peer Associations API
  slug: amazon-cloud-wan-transit-gateway-connect-peer-associations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-cloud-wan/openapi/amazon-cloud-wan-transit-gateway-connect-peer-associations-api-openapi.yml
- filename: amazon-cloud-wan-transit-gateway-registrations-api-openapi.yml
  format: yaml
  label: Amazon Cloud WAN Cloud Wan Transit Gateway Registrations API
  slug: amazon-cloud-wan-transit-gateway-registrations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-cloud-wan/openapi/amazon-cloud-wan-transit-gateway-registrations-api-openapi.yml
- filename: amazon-cloud-wan-vpc-attachments-api-openapi.yml
  format: yaml
  label: Amazon Cloud WAN Cloud Wan Vpc Attachments API
  slug: amazon-cloud-wan-vpc-attachments-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-cloud-wan/openapi/amazon-cloud-wan-vpc-attachments-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Amazon Cloud Wan Authentication
name_suffix: Authentication
oauth_flows: []
overview: Amazon Cloud WAN secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Amazon Cloud WAN
provider_slug: amazon-cloud-wan
scheme_count: 1
schemes:
- description: AWS Signature Version 4
  in: header
  name: aws_signature
  parameter: Authorization
  sources:
  - openapi/amazon-cloud-wan-openapi.yml
  type: apiKey
slug: amazon-cloud-wan-authentication
source_filename: amazon-cloud-wan-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/amazon-cloud-wan-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: aws_signature\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: AWS Signature Version 4\n  sources:\n  - openapi/amazon-cloud-wan-openapi.yml\n"
source_yaml_url: https://artifacts.apis.io/amazon-cloud-wan/authentication/amazon-cloud-wan-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Cloud WAN
- Networking
- Wide Area Network
- SD-WAN
---
