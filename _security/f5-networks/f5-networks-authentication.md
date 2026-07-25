---
api_key_in:
- header
api_specs:
- filename: f5-networks-nodes-api-openapi.yml
  format: yaml
  label: F5 Networks Nodes API
  slug: f5-networks-nodes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/f5-networks/refs/heads/main/openapi/f5-networks-nodes-api-openapi.yml
- filename: f5-networks-pool-members-api-openapi.yml
  format: yaml
  label: F5 Networks Pool Members API
  slug: f5-networks-pool-members-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/f5-networks/refs/heads/main/openapi/f5-networks-pool-members-api-openapi.yml
- filename: f5-networks-pools-api-openapi.yml
  format: yaml
  label: F5 Networks Pools API
  slug: f5-networks-pools-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/f5-networks/refs/heads/main/openapi/f5-networks-pools-api-openapi.yml
- filename: f5-networks-profiles-api-openapi.yml
  format: yaml
  label: F5 Networks Profiles API
  slug: f5-networks-profiles-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/f5-networks/refs/heads/main/openapi/f5-networks-profiles-api-openapi.yml
- filename: f5-networks-virtual-servers-api-openapi.yml
  format: yaml
  label: F5 Networks Virtual Servers API
  slug: f5-networks-virtual-servers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/f5-networks/refs/heads/main/openapi/f5-networks-virtual-servers-api-openapi.yml
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
