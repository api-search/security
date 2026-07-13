---
api_key_in:
- header
api_specs:
- filename: bigip-icontrol-rest.yml
  format: yaml
  label: F5 BIG-IP iControl REST API
  slug: f5-big-ip-icontrol-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/f5-networks/refs/heads/main/openapi/bigip-icontrol-rest.yml
- filename: swagger
  format: yaml
  label: F5 Distributed Cloud API
  slug: f5-distributed-cloud-api
  spec_type: OpenAPI
  url: https://docs.cloud.f5.com/docs/api/swagger
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: derived
name: F5 Networks Authentication
name_suffix: Authentication
oauth_flows: []
overview: F5 Networks secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: F5 Networks
provider_slug: f5-networks
scheme_count: 2
schemes:
- description: HTTP Basic authentication using BIG-IP admin credentials. The username and password are sent base64-encoded in the Authorization header.
  name: basicAuth
  scheme: basic
  sources:
  - openapi/bigip-icontrol-rest.yml
  type: http
- description: Token-based authentication. Obtain a token by POSTing credentials to /mgmt/shared/authn/login, then pass the token value in the X-F5-Auth-Token header for subsequent requests.
  in: header
  name: tokenAuth
  parameter: X-F5-Auth-Token
  sources:
  - openapi/bigip-icontrol-rest.yml
  type: apiKey
slug: f5-networks-authentication
source_filename: f5-networks-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/bigip-icontrol-rest.yml\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: basicAuth\n  type: http\n  scheme: basic\n  description: HTTP Basic authentication using BIG-IP admin credentials. The username and password\n    are sent base64-encoded in the Authorization header.\n  sources:\n  - openapi/bigip-icontrol-rest.yml\n- name: tokenAuth\n  type: apiKey\n  in: header\n  parameter: X-F5-Auth-Token\n  description: Token-based authentication. Obtain a token by POSTing credentials to /mgmt/shared/authn/login,\n    then pass the token value in the X-F5-Auth-Token header for subsequent requests.\n  sources:\n  - openapi/bigip-icontrol-rest.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/f5-networks/refs/heads/main/authentication/f5-networks-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- API Gateway
- Application Delivery
- Automation
- Edge Computing
- Kubernetes
- Load Balancing
- Multi-Cloud
- NGINX
- Security
- WAF
---
