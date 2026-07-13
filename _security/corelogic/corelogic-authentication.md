---
api_key_in: []
api_specs:
- filename: corelogic-trestle-reso-web-api-openapi.yml
  format: yaml
  label: Trestle RESO Web API
  slug: trestle-reso-web-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/corelogic/refs/heads/main/openapi/corelogic-trestle-reso-web-api-openapi.yml
- filename: corelogic-direct-webapi-crm-openapi.yml
  format: yaml
  label: Direct Web API — CRM
  slug: direct-webapi-crm
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/corelogic/refs/heads/main/openapi/corelogic-direct-webapi-crm-openapi.yml
auth_types:
- http
- oauth2
- openIdConnect
description: ''
kind: authentication
layout: security
method: derived
name: Corelogic Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: CoreLogic (Cotality) secures its APIs with http, oauth2, and openIdConnect across 3 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: CoreLogic (Cotality)
provider_slug: corelogic
scheme_count: 3
schemes:
- name: oidcClareity
  openIdConnectUrl: https://api.cotality.com/trestle/oidc/.well-known/openid-configuration
  sources:
  - openapi/corelogic-direct-webapi-crm-openapi.yml
  type: openIdConnect
- name: basicAuth
  scheme: basic
  sources:
  - openapi/corelogic-direct-webapi-crm-openapi.yml
  type: http
- flows:
  - flow: clientCredentials
    scopes: 1
    tokenUrl: https://api.cotality.com/trestle/oidc/connect/token
  name: oauth2ClientCredentials
  sources:
  - openapi/corelogic-trestle-reso-web-api-openapi.yml
  type: oauth2
slug: corelogic-authentication
source_filename: corelogic-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/corelogic-direct-webapi-crm-openapi.yml, openapi/corelogic-trestle-reso-web-api-openapi.yml\nsummary:\n  types:\n  - http\n  - oauth2\n  - openIdConnect\n  oauth2_flows:\n  - clientCredentials\nschemes:\n- name: oidcClareity\n  type: openIdConnect\n  openIdConnectUrl: https://api.cotality.com/trestle/oidc/.well-known/openid-configuration\n  sources:\n  - openapi/corelogic-direct-webapi-crm-openapi.yml\n- name: basicAuth\n  type: http\n  scheme: basic\n  sources:\n  - openapi/corelogic-direct-webapi-crm-openapi.yml\n- name: oauth2ClientCredentials\n  type: oauth2\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api.cotality.com/trestle/oidc/connect/token\n    scopes: 1\n  sources:\n  - openapi/corelogic-trestle-reso-web-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/corelogic/refs/heads/main/authentication/corelogic-authentication.yml
summary_line: http/oauth2/openIdConnect · 3 schemes
tags:
- Climate Risk
- CoreLogic
- Cotality
- Direct Web API
- Hazard Data
- Insurance Data
- Listings
- Matrix MLS
- Mortgage Data
- MLS
- OData
- OneHome
- OpenID Connect
- Participant Reporting
- Property Data
- Real Estate
- RESO Data Dictionary
- RESO Web API
- RETS
- Tax Data
- Trestle
---
