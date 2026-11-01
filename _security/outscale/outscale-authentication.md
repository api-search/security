---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: outscale-clusters-api-openapi.yml
  format: yaml
  label: 3DS OUTSCALE Clusters API
  slug: outscale-clusters-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/outscale/openapi/outscale-clusters-api-openapi.yml
- filename: outscale-myip-api-openapi.yml
  format: yaml
  label: 3DS OUTSCALE My Ip API
  slug: outscale-myip-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/outscale/openapi/outscale-myip-api-openapi.yml
- filename: outscale-projects-api-openapi.yml
  format: yaml
  label: 3DS OUTSCALE Projects API
  slug: outscale-projects-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/outscale/openapi/outscale-projects-api-openapi.yml
- filename: outscale-quotas-api-openapi.yml
  format: yaml
  label: 3DS OUTSCALE Quotas API
  slug: outscale-quotas-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/outscale/openapi/outscale-quotas-api-openapi.yml
- filename: outscale-templates-api-openapi.yml
  format: yaml
  label: 3DS OUTSCALE Templates API
  slug: outscale-templates-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/outscale/openapi/outscale-templates-api-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
mechanism_count: 6
method: derived
name: Outscale Authentication
name_suffix: Authentication
oauth_flows: []
overview: 3DS OUTSCALE secures its APIs with apiKey and http across 6 declared security schemes, as derived from its OpenAPI definitions.
provider_name: 3DS OUTSCALE
provider_slug: outscale
scheme_count: 6
schemes:
- description: Username and Password for API authentication
  name: BasicAuth
  scheme: basic
  sources:
  - openapi/outscale-oks-openapi.yml
  type: http
- description: AccessKey for API authentication
  in: header
  name: AccessKeyAuth
  parameter: AccessKey
  sources:
  - openapi/outscale-oks-openapi.yml
  type: apiKey
- description: SecretKey for API authentication
  in: header
  name: SecretKeyAuth
  parameter: SecretKey
  sources:
  - openapi/outscale-oks-openapi.yml
  type: apiKey
- description: Access Token for API authentication
  in: header
  name: AccessTokenAuth
  parameter: AccessToken
  sources:
  - openapi/outscale-oks-openapi.yml
  type: apiKey
- description: Refresh Token for API authentication
  in: header
  name: RefreshTokenAuth
  parameter: RefreshToken
  sources:
  - openapi/outscale-oks-openapi.yml
  type: apiKey
- description: OTP token for API authentication
  in: header
  name: OTPCodeAuth
  parameter: X-OTP-Code
  sources:
  - openapi/outscale-oks-openapi.yml
  type: apiKey
slug: outscale-authentication
source_filename: outscale-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-28'\nmethod: derived\nsource: openapi/outscale-oks-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: BasicAuth\n  type: http\n  scheme: basic\n  description: Username and Password for API authentication\n  sources:\n  - openapi/outscale-oks-openapi.yml\n- name: AccessKeyAuth\n  type: apiKey\n  in: header\n  parameter: AccessKey\n  description: AccessKey for API authentication\n  sources:\n  - openapi/outscale-oks-openapi.yml\n- name: SecretKeyAuth\n  type: apiKey\n  in: header\n  parameter: SecretKey\n  description: SecretKey for API authentication\n  sources:\n  - openapi/outscale-oks-openapi.yml\n- name: AccessTokenAuth\n  type: apiKey\n  in: header\n  parameter: AccessToken\n  description: Access Token for API authentication\n  sources:\n  - openapi/outscale-oks-openapi.yml\n- name: RefreshTokenAuth\n  type: apiKey\n  in: header\n  parameter: RefreshToken\n  description: Refresh Token for API authentication\n\
  \  sources:\n  - openapi/outscale-oks-openapi.yml\n- name: OTPCodeAuth\n  type: apiKey\n  in: header\n  parameter: X-OTP-Code\n  description: OTP token for API authentication\n  sources:\n  - openapi/outscale-oks-openapi.yml\n"
source_yaml_url: https://artifacts.apis.io/outscale/authentication/outscale-authentication.yml
summary_line: apiKey/http · 6 schemes
tags:
- Cloud
- IaaS
- Compute
- Storage
- Networking
---
