---
anonymous_access: false
api_key_in: []
auth_types:
- oauth2
- http
- custom-token
description: ''
kind: authentication
layout: security
mechanism_count: 4
method: searched
name: Ge Vernova Authentication
name_suffix: Authentication
oauth_flows:
- password
- clientCredentials
- authorizationCode
overview: GE Vernova secures its APIs with oauth2, http, and custom-token across 4 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the password, clientCredentials, and authorizationCode flow(s).
provider_name: GE Vernova
provider_slug: ge-vernova
scheme_count: 4
schemes:
- description: Proficy Authentication (UAA) provides identity-based security for Proficy applications. REST clients obtain a bearer token from the UAA token endpoint and present it to the product's REST service; the Swagger UI shipped with each product authorizes against the same service.
  flows:
  - flow: password
    note: Historian's own documentation shows the Swagger UI authorizing with the oauth2schema (OAuth2, password) section using client_id historian_public_rest_api.
  - flow: clientCredentials
    note: clients are created and granted authorities/scopes in Proficy Authentication
  name: ProficyAuthentication
  product: Proficy Historian / Plant Applications / Operations Hub / iFIX
  scopes_reference: scopes/ge-vernova-scopes.yml
  source: https://www.gevernova.com/software/documentation/uaa/version2025/index.html
  type: oauth2
- description: APM OData and ingestion requests are authenticated against Predix UAA. Two calls are required — an HTTP POST to {{uaa-uri}}/oauth/token with grant_type=password and a Basic authorization header, then the API call with the resulting access token. APM's docs state explicitly that SSO credentials cannot be used for OData; a UAA account is required.
  flows:
  - flow: password
    tokenUrl: '{{uaa-uri}}/oauth/token'
  name: PredixUAA
  product: Cloud APM (OData data-extraction API, Simple Ingestion API)
  source: https://www.gevernova.com/software/documentation/cloud-apm/latest/ade-authentication.html
  type: oauth2
- description: The Operations Hub integration APIs use a product-specific login rather than OAuth. A client POSTs {"username":"<user>","password":"<pass>"} to https://<Operations Hub_Site_URL>/app/iqp/api/rest/login and receives {"code":"1","token":"<token>"}; the token is then passed in the body of every subsequent integration call.
  name: OperationsHubIntegrationToken
  product: Proficy Operations Hub integration REST APIs
  source: https://www.gevernova.com/software/documentation/opshub/version2025/windows/r_rest_integration_apis.html
  type: custom-token
- artifact: well-known/ge-vernova-openid-configuration.json
  description: softwaresupport.gevernova.com publishes an OpenID Connect discovery document at /.well-known/openid-configuration whose issuer is the same host. It is the customer/partner sign-in for the support portal, not a product API authorization server.
  name: SupportPortalOIDC
  openIdConnectUrl: https://softwaresupport.gevernova.com/.well-known/openid-configuration
  product: GE Vernova software support portal
  type: openIdConnect
slug: ge-vernova-authentication
source_filename: ge-vernova-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-12'\nmethod: searched\nsource: >-\n  https://www.gevernova.com/software/documentation/uaa/version2025/index.html\ndocs:\n  - https://www.gevernova.com/software/documentation/uaa/version2025/index.html\n  - https://www.gevernova.com/software/documentation/historian/version2025/t_historian_swagger_documentation.html\n  - https://www.gevernova.com/software/documentation/cloud-apm/latest/ade-authentication.html\n  - https://www.gevernova.com/software/documentation/opshub/version2025/windows/r_rest_integration_apis.html\nnote: >-\n  No OpenAPI/Swagger document is published for any GE Vernova Electrification Software product —\n  each product's Swagger UI is served from the customer's own installed instance — so this profile\n  is read from the published documentation rather than derived from a spec.\nsummary:\n  types: [oauth2, http, custom-token]\n  api_key_in: []\n  oauth2_flows: [password, clientCredentials, authorizationCode]\n  identity_provider: Proficy\
  \ Authentication (Cloud Foundry UAA) for on-premises Proficy products; Predix UAA for Cloud APM\nschemes:\n  - name: ProficyAuthentication\n    type: oauth2\n    product: Proficy Historian / Plant Applications / Operations Hub / iFIX\n    description: >-\n      Proficy Authentication (UAA) provides identity-based security for Proficy applications. REST\n      clients obtain a bearer token from the UAA token endpoint and present it to the product's\n      REST service; the Swagger UI shipped with each product authorizes against the same service.\n    flows:\n      - flow: password\n        note: >-\n          Historian's own documentation shows the Swagger UI authorizing with the oauth2schema\n          (OAuth2, password) section using client_id historian_public_rest_api.\n      - flow: clientCredentials\n        note: clients are created and granted authorities/scopes in Proficy Authentication\n    scopes_reference: scopes/ge-vernova-scopes.yml\n    source: https://www.gevernova.com/software/documentation/uaa/version2025/index.html\n\
  \  - name: PredixUAA\n    type: oauth2\n    product: Cloud APM (OData data-extraction API, Simple Ingestion API)\n    description: >-\n      APM OData and ingestion requests are authenticated against Predix UAA. Two calls are\n      required — an HTTP POST to {{uaa-uri}}/oauth/token with grant_type=password and a Basic\n      authorization header, then the API call with the resulting access token. APM's docs state\n      explicitly that SSO credentials cannot be used for OData; a UAA account is required.\n    flows:\n      - flow: password\n        tokenUrl: '{{uaa-uri}}/oauth/token'\n    source: https://www.gevernova.com/software/documentation/cloud-apm/latest/ade-authentication.html\n  - name: OperationsHubIntegrationToken\n    type: custom-token\n    product: Proficy Operations Hub integration REST APIs\n    description: >-\n      The Operations Hub integration APIs use a product-specific login rather than OAuth. A client\n      POSTs {\"username\":\"<user>\",\"password\":\"<pass>\"\
  } to\n      https://<Operations Hub_Site_URL>/app/iqp/api/rest/login and receives {\"code\":\"1\",\"token\":\"<token>\"};\n      the token is then passed in the body of every subsequent integration call.\n    source: https://www.gevernova.com/software/documentation/opshub/version2025/windows/r_rest_integration_apis.html\n  - name: SupportPortalOIDC\n    type: openIdConnect\n    product: GE Vernova software support portal\n    description: >-\n      softwaresupport.gevernova.com publishes an OpenID Connect discovery document at\n      /.well-known/openid-configuration whose issuer is the same host. It is the customer/partner\n      sign-in for the support portal, not a product API authorization server.\n    openIdConnectUrl: https://softwaresupport.gevernova.com/.well-known/openid-configuration\n    artifact: well-known/ge-vernova-openid-configuration.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ge-vernova/refs/heads/main/authentication/ge-vernova-authentication.yml
summary_line: oauth2/http/custom-token · 4 schemes
tags:
- Decarbonization
- Electrification
- Energy
- Fortune 500
- Power
- Renewable Energy
- Sustainability
- Industrial
- Asset Performance Management
- Manufacturing Execution Systems
- Historian
- Grid
---
