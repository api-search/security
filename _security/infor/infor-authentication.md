---
anonymous_access: false
api_key_in: []
api_specs:
- filename: infor-contents-api-openapi.yml
  format: yaml
  label: Infor Contents API
  slug: infor-contents-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/infor/openapi/infor-contents-api-openapi.yml
- filename: infor-icua-api-openapi.yml
  format: yaml
  label: Infor ICUA API
  slug: infor-icua-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/infor/openapi/infor-icua-api-openapi.yml
- filename: infor-languages-api-openapi.yml
  format: yaml
  label: Infor Languages API
  slug: infor-languages-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/infor/openapi/infor-languages-api-openapi.yml
- filename: infor-products-api-openapi.yml
  format: yaml
  label: Infor Products API
  slug: infor-products-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/infor/openapi/infor-products-api-openapi.yml
- filename: infor-recenttopics-api-openapi.yml
  format: yaml
  label: Infor Recent Topics API
  slug: infor-recenttopics-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/infor/openapi/infor-recenttopics-api-openapi.yml
- filename: infor-s3-docs-api-openapi.yml
  format: yaml
  label: Infor S3 Docs API
  slug: infor-s3-docs-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/infor/openapi/infor-s3-docs-api-openapi.yml
- filename: infor-search-api-openapi.yml
  format: yaml
  label: Infor Search API
  slug: infor-search-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/infor/openapi/infor-search-api-openapi.yml
- filename: infor-security-api-openapi.yml
  format: yaml
  label: Infor Security API
  slug: infor-security-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/infor/openapi/infor-security-api-openapi.yml
- filename: infor-solutions-api-openapi.yml
  format: yaml
  label: Infor Solutions API
  slug: infor-solutions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/infor/openapi/infor-solutions-api-openapi.yml
- filename: infor-userfavorites-api-openapi.yml
  format: yaml
  label: Infor User Favorites API
  slug: infor-userfavorites-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/infor/openapi/infor-userfavorites-api-openapi.yml
- filename: infor-web-api-openapi.yml
  format: yaml
  label: Infor Web API
  slug: infor-web-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/infor/openapi/infor-web-api-openapi.yml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: derived
name: Infor Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- clientCredentials
overview: Infor secures its APIs with oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode and clientCredentials flow(s).
provider_name: Infor
provider_slug: infor
scheme_count: 2
schemes:
- description: Infor ION API Client Credentials grant
  flows:
  - flow: clientCredentials
    scopes: 0
    tokenUrl: https://inforos.infor.com/INFOR_DEV/as/token.oauth2
  name: OAuth2ClientCredentials
  sources:
  - openapi/infor-ion-documents-api-openapi.yml
  - openapi/infor-m3-api-api-openapi.yml
  type: oauth2
- description: Infor ION API Authorization Code grant
  flows:
  - authorizationUrl: https://inforos.infor.com/INFOR_DEV/as/authorization.oauth2
    flow: authorizationCode
    scopes: 0
    tokenUrl: https://inforos.infor.com/INFOR_DEV/as/token.oauth2
  name: OAuth2AuthorizationCode
  sources:
  - openapi/infor-ion-documents-api-openapi.yml
  - openapi/infor-m3-api-api-openapi.yml
  type: oauth2
slug: infor-authentication
source_filename: infor-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-13'\nmethod: derived\nsource: openapi/infor-ion-documents-api-openapi.yml, openapi/infor-m3-api-api-openapi.yml\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\n  - clientCredentials\nschemes:\n- name: OAuth2ClientCredentials\n  type: oauth2\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://inforos.infor.com/INFOR_DEV/as/token.oauth2\n    scopes: 0\n  description: Infor ION API Client Credentials grant\n  sources:\n  - openapi/infor-ion-documents-api-openapi.yml\n  - openapi/infor-m3-api-api-openapi.yml\n- name: OAuth2AuthorizationCode\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://inforos.infor.com/INFOR_DEV/as/authorization.oauth2\n    tokenUrl: https://inforos.infor.com/INFOR_DEV/as/token.oauth2\n    scopes: 0\n  description: Infor ION API Authorization Code grant\n  sources:\n  - openapi/infor-ion-documents-api-openapi.yml\n  - openapi/infor-m3-api-api-openapi.yml\n"
source_yaml_url: https://artifacts.apis.io/infor/authentication/infor-authentication.yml
summary_line: oauth2 · 2 schemes
tags:
- ERP
- Manufacturing
- Supply Chain
- Cloud
- Integration
---
