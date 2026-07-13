---
api_key_in:
- cookie
api_specs:
- filename: isg-rest-api.yml
  format: yaml
  label: Oracle EBS Integrated SOA Gateway REST API
  slug: oracle-ebs-integrated-soa-gateway-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/oracle-e-business-suite/refs/heads/main/openapi/isg-rest-api.yml
- filename: financial-services-api.yml
  format: yaml
  label: Oracle EBS Financial Services API
  slug: oracle-ebs-financial-services-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/oracle-e-business-suite/refs/heads/main/openapi/financial-services-api.yml
- filename: supply-chain-api.yml
  format: yaml
  label: Oracle EBS Supply Chain Management API
  slug: oracle-ebs-supply-chain-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/oracle-e-business-suite/refs/heads/main/openapi/supply-chain-api.yml
- filename: human-resources-api.yml
  format: yaml
  label: Oracle EBS Human Resources API
  slug: oracle-ebs-human-resources-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/oracle-e-business-suite/refs/heads/main/openapi/human-resources-api.yml
- filename: manufacturing-api.yml
  format: yaml
  label: Oracle EBS Manufacturing API
  slug: oracle-ebs-manufacturing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/oracle-e-business-suite/refs/heads/main/openapi/manufacturing-api.yml
- filename: ecommerce-gateway-api.yml
  format: yaml
  label: Oracle EBS e-Commerce Gateway API
  slug: oracle-ebs-e-commerce-gateway-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/oracle-e-business-suite/refs/heads/main/openapi/ecommerce-gateway-api.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: derived
name: Oracle E Business Suite Authentication
name_suffix: Authentication
oauth_flows: []
overview: Oracle E-Business Suite secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Oracle E-Business Suite
provider_slug: oracle-e-business-suite
scheme_count: 2
schemes:
- description: HTTP Basic Authentication with Oracle EBS username and password
  name: basicAuth
  scheme: basic
  sources:
  - openapi/ecommerce-gateway-api.yml
  - openapi/financial-services-api.yml
  - openapi/human-resources-api.yml
  - openapi/isg-rest-api.yml
  - openapi/manufacturing-api.yml
  - openapi/supply-chain-api.yml
  type: http
- description: Token-based authentication using the ISG login access token
  in: cookie
  name: tokenAuth
  parameter: accessToken
  sources:
  - openapi/ecommerce-gateway-api.yml
  - openapi/financial-services-api.yml
  - openapi/human-resources-api.yml
  - openapi/isg-rest-api.yml
  - openapi/manufacturing-api.yml
  - openapi/supply-chain-api.yml
  type: apiKey
slug: oracle-e-business-suite-authentication
source_filename: oracle-e-business-suite-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/ecommerce-gateway-api.yml, openapi/financial-services-api.yml, openapi/human-resources-api.yml,\n  openapi/isg-rest-api.yml, openapi/manufacturing-api.yml, openapi/supply-chain-api.yml\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - cookie\nschemes:\n- name: basicAuth\n  type: http\n  scheme: basic\n  description: HTTP Basic Authentication with Oracle EBS username and password\n  sources:\n  - openapi/ecommerce-gateway-api.yml\n  - openapi/financial-services-api.yml\n  - openapi/human-resources-api.yml\n  - openapi/isg-rest-api.yml\n  - openapi/manufacturing-api.yml\n  - openapi/supply-chain-api.yml\n- name: tokenAuth\n  type: apiKey\n  in: cookie\n  parameter: accessToken\n  description: Token-based authentication using the ISG login access token\n  sources:\n  - openapi/ecommerce-gateway-api.yml\n  - openapi/financial-services-api.yml\n  - openapi/human-resources-api.yml\n  - openapi/isg-rest-api.yml\n\
  \  - openapi/manufacturing-api.yml\n  - openapi/supply-chain-api.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/oracle-e-business-suite/refs/heads/main/authentication/oracle-e-business-suite-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Business Applications
- E-Business Suite
- Enterprise
- ERP
- Oracle
---
