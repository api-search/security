---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: amazon-network-firewall-aws-network-firewall-api-openapi.yml
  format: yaml
  label: Amazon Network Firewall AWS Network Firewall API
  slug: amazon-network-firewall-aws-network-firewall-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-network-firewall/openapi/amazon-network-firewall-aws-network-firewall-api-openapi.yml
- filename: amazon-network-firewall-network-firewall-transit-gateway-attachment-api-openapi.yml
  format: yaml
  label: Amazon Network Firewall Network Firewall Network Firewall Transit Gateway Attachment API
  slug: amazon-network-firewall-network-firewall-transit-gateway-attachment-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-network-firewall/openapi/amazon-network-firewall-network-firewall-transit-gateway-attachment-api-openapi.yml
- filename: amazon-network-firewall-container-association-api-openapi.yml
  format: yaml
  label: Amazon Network Firewall Network Firewall Container Association API
  slug: amazon-network-firewall-container-association-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-network-firewall/openapi/amazon-network-firewall-container-association-api-openapi.yml
- filename: amazon-network-firewall-operations-api-openapi.yml
  format: yaml
  label: Amazon Network Firewall Network Firewall Operations API
  slug: amazon-network-firewall-operations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-network-firewall/openapi/amazon-network-firewall-operations-api-openapi.yml
- filename: amazon-network-firewall-proxy-api-openapi.yml
  format: yaml
  label: Amazon Network Firewall Network Firewall Proxy API
  slug: amazon-network-firewall-proxy-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-network-firewall/openapi/amazon-network-firewall-proxy-api-openapi.yml
- filename: amazon-network-firewall-proxy-configuration-api-openapi.yml
  format: yaml
  label: Amazon Network Firewall Network Firewall Proxy Configuration API
  slug: amazon-network-firewall-proxy-configuration-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-network-firewall/openapi/amazon-network-firewall-proxy-configuration-api-openapi.yml
- filename: amazon-network-firewall-proxy-rule-api-openapi.yml
  format: yaml
  label: Amazon Network Firewall Network Firewall Proxy Rule API
  slug: amazon-network-firewall-proxy-rule-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-network-firewall/openapi/amazon-network-firewall-proxy-rule-api-openapi.yml
- filename: amazon-network-firewall-proxy-rule-group-api-openapi.yml
  format: yaml
  label: Amazon Network Firewall Network Firewall Proxy Rule Group API
  slug: amazon-network-firewall-proxy-rule-group-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-network-firewall/openapi/amazon-network-firewall-proxy-rule-group-api-openapi.yml
- filename: amazon-network-firewall-vpc-endpoint-association-api-openapi.yml
  format: yaml
  label: Amazon Network Firewall Network Firewall Vpc Endpoint Association API
  slug: amazon-network-firewall-vpc-endpoint-association-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-network-firewall/openapi/amazon-network-firewall-vpc-endpoint-association-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Amazon Network Firewall Authentication
name_suffix: Authentication
oauth_flows: []
overview: Amazon Network Firewall secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Amazon Network Firewall
provider_slug: amazon-network-firewall
scheme_count: 1
schemes:
- description: Amazon Signature authorization v4
  in: header
  name: hmac
  parameter: Authorization
  sources:
  - openapi/amazon-network-firewall-openapi.yml
  type: apiKey
slug: amazon-network-firewall-authentication
source_filename: amazon-network-firewall-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/amazon-network-firewall-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: hmac\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: Amazon Signature authorization v4\n  sources:\n  - openapi/amazon-network-firewall-openapi.yml\n"
source_yaml_url: https://artifacts.apis.io/amazon-network-firewall/authentication/amazon-network-firewall-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Firewall
- Intrusion Detection
- Network Security
- VPC
---
