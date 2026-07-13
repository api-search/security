---
api_key_in:
- header
api_specs:
- filename: f5-load-balancer-icontrol-rest-openapi.yml
  format: yaml
  label: F5 BIG-IP iControl REST API
  slug: f5-bigip-icontrol-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/f5-load-balancer/refs/heads/main/openapi/f5-load-balancer-icontrol-rest-openapi.yml
- filename: f5-load-balancer-as3-openapi.yml
  format: yaml
  label: F5 BIG-IP AS3 API
  slug: f5-bigip-as3-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/f5-load-balancer/refs/heads/main/openapi/f5-load-balancer-as3-openapi.yml
- filename: f5-load-balancer-declarative-onboarding-openapi.yml
  format: yaml
  label: F5 BIG-IP Declarative Onboarding API
  slug: f5-bigip-declarative-onboarding-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/f5-load-balancer/refs/heads/main/openapi/f5-load-balancer-declarative-onboarding-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: derived
name: F5 Load Balancer Authentication
name_suffix: Authentication
oauth_flows: []
overview: F5 Load Balancer secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: F5 Load Balancer
provider_slug: f5-load-balancer
scheme_count: 2
schemes:
- description: HTTP Basic Authentication using BIG-IP admin credentials.
  name: basicAuth
  scheme: basic
  sources:
  - openapi/f5-load-balancer-as3-openapi.yml
  - openapi/f5-load-balancer-declarative-onboarding-openapi.yml
  - openapi/f5-load-balancer-icontrol-rest-openapi.yml
  type: http
- description: Token-based authentication obtained from the /mgmt/shared/authn/login endpoint.
  in: header
  name: tokenAuth
  parameter: X-F5-Auth-Token
  sources:
  - openapi/f5-load-balancer-as3-openapi.yml
  - openapi/f5-load-balancer-declarative-onboarding-openapi.yml
  - openapi/f5-load-balancer-icontrol-rest-openapi.yml
  type: apiKey
slug: f5-load-balancer-authentication
source_filename: f5-load-balancer-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/f5-load-balancer-as3-openapi.yml, openapi/f5-load-balancer-declarative-onboarding-openapi.yml,\n  openapi/f5-load-balancer-icontrol-rest-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: basicAuth\n  type: http\n  scheme: basic\n  description: HTTP Basic Authentication using BIG-IP admin credentials.\n  sources:\n  - openapi/f5-load-balancer-as3-openapi.yml\n  - openapi/f5-load-balancer-declarative-onboarding-openapi.yml\n  - openapi/f5-load-balancer-icontrol-rest-openapi.yml\n- name: tokenAuth\n  type: apiKey\n  in: header\n  parameter: X-F5-Auth-Token\n  description: Token-based authentication obtained from the /mgmt/shared/authn/login endpoint.\n  sources:\n  - openapi/f5-load-balancer-as3-openapi.yml\n  - openapi/f5-load-balancer-declarative-onboarding-openapi.yml\n  - openapi/f5-load-balancer-icontrol-rest-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/f5-load-balancer/refs/heads/main/authentication/f5-load-balancer-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Application Delivery
- BIG-IP
- Load Balancer
- Networking
- Traffic Management
---
