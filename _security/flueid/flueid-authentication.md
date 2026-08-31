---
api_key_in: []
api_specs:
- filename: flueid-account-api-openapi.yml
  format: yaml
  label: Flueid Account API
  slug: flueid-account-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/flueid/refs/heads/main/openapi/flueid-account-api-openapi.yml
- filename: flueid-accountpartner-api-openapi.yml
  format: yaml
  label: Flueid Account Partner API
  slug: flueid-accountpartner-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/flueid/refs/heads/main/openapi/flueid-accountpartner-api-openapi.yml
- filename: flueid-clientcompanies-api-openapi.yml
  format: yaml
  label: Flueid Client Companies API
  slug: flueid-clientcompanies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/flueid/refs/heads/main/openapi/flueid-clientcompanies-api-openapi.yml
- filename: flueid-documents-api-openapi.yml
  format: yaml
  label: Flueid Documents API
  slug: flueid-documents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/flueid/refs/heads/main/openapi/flueid-documents-api-openapi.yml
- filename: flueid-farms-api-openapi.yml
  format: yaml
  label: Flueid Farms API
  slug: flueid-farms-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/flueid/refs/heads/main/openapi/flueid-farms-api-openapi.yml
- filename: flueid-neworders-api-openapi.yml
  format: yaml
  label: Flueid New Orders API
  slug: flueid-neworders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/flueid/refs/heads/main/openapi/flueid-neworders-api-openapi.yml
- filename: flueid-orderdocumentsettings-api-openapi.yml
  format: yaml
  label: Flueid Order Document Settings API
  slug: flueid-orderdocumentsettings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/flueid/refs/heads/main/openapi/flueid-orderdocumentsettings-api-openapi.yml
- filename: flueid-orderevents-api-openapi.yml
  format: yaml
  label: Flueid Order Events API
  slug: flueid-orderevents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/flueid/refs/heads/main/openapi/flueid-orderevents-api-openapi.yml
- filename: flueid-orderoptions-api-openapi.yml
  format: yaml
  label: Flueid Order Options API
  slug: flueid-orderoptions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/flueid/refs/heads/main/openapi/flueid-orderoptions-api-openapi.yml
- filename: flueid-orders-api-openapi.yml
  format: yaml
  label: Flueid Orders API
  slug: flueid-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/flueid/refs/heads/main/openapi/flueid-orders-api-openapi.yml
- filename: flueid-partnerordersettings-api-openapi.yml
  format: yaml
  label: Flueid Partner Order Settings API
  slug: flueid-partnerordersettings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/flueid/refs/heads/main/openapi/flueid-partnerordersettings-api-openapi.yml
- filename: flueid-partners-api-openapi.yml
  format: yaml
  label: Flueid Partners API
  slug: flueid-partners-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/flueid/refs/heads/main/openapi/flueid-partners-api-openapi.yml
- filename: flueid-permissions-api-openapi.yml
  format: yaml
  label: Flueid Permissions API
  slug: flueid-permissions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/flueid/refs/heads/main/openapi/flueid-permissions-api-openapi.yml
- filename: flueid-propertydata-api-openapi.yml
  format: yaml
  label: Flueid Property Data API
  slug: flueid-propertydata-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/flueid/refs/heads/main/openapi/flueid-propertydata-api-openapi.yml
- filename: flueid-public-api-openapi.yml
  format: yaml
  label: Flueid Public API
  slug: flueid-public-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/flueid/refs/heads/main/openapi/flueid-public-api-openapi.yml
- filename: flueid-settings-api-openapi.yml
  format: yaml
  label: Flueid Settings API
  slug: flueid-settings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/flueid/refs/heads/main/openapi/flueid-settings-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: searched
name: Flueid Authentication
name_suffix: Authentication
oauth_flows: []
overview: Flueid secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Flueid
provider_slug: flueid
scheme_count: 1
schemes:
- bearerFormat: JWT
  header: 'Authorization: Bearer <jwt>'
  issuer: Amazon Cognito user pool (AWS Amplify auth), region us-east-1/us-west-2 pools referenced in the client bundle
  name: bearerAuth
  note: Observed in the Flueid Pro client bundle, which uses AWS Amplify Auth (CognitoUser, UserPoolId, IdentityPoolId, cognitoClientId) and attaches an Authorization header to every api.pro.flueid.com request.
  scheme: bearer
  sources:
  - https://pro.flueid.com/static/js/main.e47cfca1.js
  type: http
slug: flueid-authentication
source_filename: flueid-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-16'\nmethod: searched\nsource: https://pro.flueid.com/static/js/main.e47cfca1.js + https://www.flueid.com/security\ndocs: null\nsummary:\n  types:\n  - http\n  http_schemes:\n  - bearer\n  api_key_in: []\n  oauth2_flows: []\n  declared_in_openapi: false\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  sources:\n  - https://pro.flueid.com/static/js/main.e47cfca1.js\n  issuer: Amazon Cognito user pool (AWS Amplify auth), region us-east-1/us-west-2 pools referenced in\n    the client bundle\n  header: 'Authorization: Bearer <jwt>'\n  note: Observed in the Flueid Pro client bundle, which uses AWS Amplify Auth (CognitoUser, UserPoolId,\n    IdentityPoolId, cognitoClientId) and attaches an Authorization header to every api.pro.flueid.com\n    request.\ngaps:\n- The published OpenAPI declares no components.securitySchemes at all, so an agent reading the contract\n  cannot tell how to authenticate.\n- No /.well-known/openid-configuration\
  \ or /.well-known/oauth-authorization-server is served on any Flueid\n  host.\n- No public authentication documentation page exists; Flueid publishes no developer portal.\nprovider_claim: 'Flueid states on https://www.flueid.com/security: \"Our VOT platform APIs securely exchange\n  data between systems using leading token-based authentication and dedicated KMS encryption management.\"'\nx-evidence:\n- url: https://api.pro.flueid.com/swagger/v1/swagger.json\n  http_status: 200\n  note: components.securitySchemes is empty\n- url: https://api.pro.flueid.com/.well-known/openid-configuration\n  http_status: 404\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/flueid/refs/heads/main/authentication/flueid-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Real-Estate
- Title Insurance
- Mortgage
- Property Data
- Verification of Title
- Financial-Services
- Lending
- PropTech
- Settlement Services
---
