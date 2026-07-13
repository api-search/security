---
api_key_in: []
api_specs:
- filename: api-rest-api.html
  format: yaml
  label: Oracle Fusion ERP REST API
  slug: oracle-fusion-erp-rest-api
  spec_type: OpenAPI
  url: https://docs.oracle.com/en/cloud/saas/financials/22r3/farfa/api-rest-api.html
- filename: api-rest-api.html
  format: yaml
  label: Oracle Fusion HCM REST API
  slug: oracle-fusion-hcm-rest-api
  spec_type: OpenAPI
  url: https://docs.oracle.com/en/cloud/saas/human-resources/22r3/farws/api-rest-api.html
- filename: api-rest-api.html
  format: yaml
  label: Oracle Fusion SCM REST API
  slug: oracle-fusion-scm-rest-api
  spec_type: OpenAPI
  url: https://docs.oracle.com/en/cloud/saas/supply-chain-management/22r3/fasrs/api-rest-api.html
- filename: rest-api.html
  format: yaml
  label: Oracle Fusion CX Sales and Fusion Service REST API
  slug: oracle-fusion-cx-sales-and-fusion-service-rest-api
  spec_type: OpenAPI
  url: https://docs.oracle.com/en/cloud/saas/cx-sales/rest-api.html
- filename: oracle-fusion-common-openapi.yml
  format: yaml
  label: Oracle Fusion Common Features REST API
  slug: oracle-fusion-common-features-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/oracle-fusion/refs/heads/main/openapi/oracle-fusion-common-openapi.yml
- filename: oracle-fusion-project-management-openapi.yml
  format: yaml
  label: Oracle Fusion Project Management REST API
  slug: oracle-fusion-project-management-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/oracle-fusion/refs/heads/main/openapi/oracle-fusion-project-management-openapi.yml
- filename: oracle-fusion-epm-openapi.yml
  format: yaml
  label: Oracle Fusion EPM REST API
  slug: oracle-fusion-epm-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/oracle-fusion/refs/heads/main/openapi/oracle-fusion-epm-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Oracle Fusion Authentication
name_suffix: Authentication
oauth_flows: []
overview: Oracle Fusion Cloud Applications secures its APIs with http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Oracle Fusion Cloud Applications
provider_slug: oracle-fusion
scheme_count: 2
schemes:
- bearerFormat: JWT
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/oracle-fusion-common-openapi.yml
  - openapi/oracle-fusion-cx-sales-openapi.yml
  - openapi/oracle-fusion-epm-openapi.yml
  - openapi/oracle-fusion-erp-openapi.yml
  - openapi/oracle-fusion-hcm-openapi.yml
  - openapi/oracle-fusion-project-management-openapi.yml
  - openapi/oracle-fusion-scm-openapi.yml
  type: http
- name: basicAuth
  scheme: basic
  sources:
  - openapi/oracle-fusion-common-openapi.yml
  - openapi/oracle-fusion-cx-sales-openapi.yml
  - openapi/oracle-fusion-epm-openapi.yml
  - openapi/oracle-fusion-erp-openapi.yml
  - openapi/oracle-fusion-hcm-openapi.yml
  - openapi/oracle-fusion-project-management-openapi.yml
  - openapi/oracle-fusion-scm-openapi.yml
  type: http
slug: oracle-fusion-authentication
source_filename: oracle-fusion-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/oracle-fusion-common-openapi.yml, openapi/oracle-fusion-cx-sales-openapi.yml,\n  openapi/oracle-fusion-epm-openapi.yml, openapi/oracle-fusion-erp-openapi.yml, openapi/oracle-fusion-hcm-openapi.yml,\n  openapi/oracle-fusion-project-management-openapi.yml, openapi/oracle-fusion-scm-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  sources:\n  - openapi/oracle-fusion-common-openapi.yml\n  - openapi/oracle-fusion-cx-sales-openapi.yml\n  - openapi/oracle-fusion-epm-openapi.yml\n  - openapi/oracle-fusion-erp-openapi.yml\n  - openapi/oracle-fusion-hcm-openapi.yml\n  - openapi/oracle-fusion-project-management-openapi.yml\n  - openapi/oracle-fusion-scm-openapi.yml\n- name: basicAuth\n  type: http\n  scheme: basic\n  sources:\n  - openapi/oracle-fusion-common-openapi.yml\n  - openapi/oracle-fusion-cx-sales-openapi.yml\n  - openapi/oracle-fusion-epm-openapi.yml\n\
  \  - openapi/oracle-fusion-erp-openapi.yml\n  - openapi/oracle-fusion-hcm-openapi.yml\n  - openapi/oracle-fusion-project-management-openapi.yml\n  - openapi/oracle-fusion-scm-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/oracle-fusion/refs/heads/main/authentication/oracle-fusion-authentication.yml
summary_line: http · 2 schemes
tags:
- Cloud
- CX
- Enterprise
- EPM
- ERP
- HCM
- Project Management
- REST API
- SaaS
- SCM
---
