---
api_key_in: []
api_specs:
- filename: kargo-public-graphql.postman_collection.json
  format: json
  label: Kargo Public GraphQL API
  slug: kargo-public-graphql-api
  spec_type: Postman
  url: https://raw.githubusercontent.com/api-evangelist/kargo/refs/heads/main/postman/kargo-public-graphql.postman_collection.json
- filename: kargo-documents-api-openapi.yml
  format: yaml
  label: Kargo Documents API
  slug: kargo-documents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kargo/refs/heads/main/openapi/kargo-documents-api-openapi.yml
- filename: kargo-sku-master-api-openapi.yml
  format: yaml
  label: Kargo SKU Master API
  slug: kargo-sku-master-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kargo/refs/heads/main/openapi/kargo-sku-master-api-openapi.yml
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Kargo Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: Kargo secures its APIs with http and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: Kargo
provider_slug: kargo
scheme_count: 2
schemes:
- name: bearerAuth
  note: Declared in the OpenAPI as a bare HTTP bearer scheme; the bearer value is an Auth0-issued JWT obtained through the client-credentials grant below.
  scheme: bearer
  sources:
  - openapi/kargo-document-intake-openapi.yml
  type: http
- flows:
  - audience: https://api.kargo.zone/public_graphql
    flow: clientCredentials
    scopes: {}
    tokenUrl: https://mykargo.us.auth0.com/oauth/token
  name: auth0-client-credentials
  sources:
  - https://docs.kargo.ai/authentication
  - well-known/kargo-openid-configuration.json
  type: oauth2
slug: kargo-authentication
source_filename: kargo-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-23'\nmethod: searched\nsource: https://docs.kargo.ai/authentication\ndocs: https://docs.kargo.ai/authentication\nsummary:\n  types:\n  - http\n  - oauth2\n  api_key_in: []\n  oauth2_flows:\n  - clientCredentials\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  sources:\n  - openapi/kargo-document-intake-openapi.yml\n  note: 'Declared in the OpenAPI as a bare HTTP bearer scheme; the bearer value is\n    an Auth0-issued JWT obtained through the client-credentials grant below.'\n- name: auth0-client-credentials\n  type: oauth2\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://mykargo.us.auth0.com/oauth/token\n    audience: https://api.kargo.zone/public_graphql\n    scopes: {}\n  sources:\n  - https://docs.kargo.ai/authentication\n  - well-known/kargo-openid-configuration.json\nauthorization_server:\n  issuer: https://mykargo.us.auth0.com/\n  vendor: Auth0\n  discovery: well-known/kargo-openid-configuration.json\n  jwks_uri: https://mykargo.us.auth0.com/.well-known/jwks.json\n\
  \  note: 'mykargo.us.auth0.com is Kargo''s own Auth0 tenant; Kargo''s authentication\n    documentation names this exact token endpoint and audience.'\ncredentials:\n  issued_by: Kargo (client_id and client_secret are created and provided by Kargo\n    to each customer; there is no self-service key issuance)\n  fields:\n  - name: Business Slug\n    description: Customer business identifier used on every request payload.\n  - name: Facility Slug\n    description: Customer facility identifier used on every request payload.\n  - name: API Client ID\n    description: Auth0 client_id, created and provided by Kargo.\n  - name: API Client Secret\n    description: Auth0 client_secret, created and provided by Kargo.\nrequest_header: 'Authorization: Bearer <bearer_token>'\ntoken_lifetime:\n  documented: 'Tokens are valid for 24 hours (docs example returns expires_in 86400);\n    the docs instruct callers to cache the token and use expires_in to decide when\n    to refresh.'\n  source: https://docs.kargo.ai/basic_examples\n\
  webhook_authentication:\n  direction: Kargo -> customer\n  scheme: HTTP Basic\n  header: 'Authorization: Basic <password>'\n  source: https://docs.kargo.ai/webhooks/shipment\nunauthenticated_surface:\n- surface: GraphQL introspection\n  endpoint: https://api.kargo.zone/public_graphql\n  observed: '2026-08-23'\n  note: 'Anonymous POST of a full __schema introspection query returned HTTP 200 and\n    the complete schema; data queries still require a bearer token.'\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/kargo/refs/heads/main/authentication/kargo-authentication.yml
summary_line: http/oauth2 · 2 schemes
tags:
- Company
- Logistics
- Supply Chain
- Warehouse
- Computer-Vision
- Artificial Intelligence
- Shipping
- Inventory
- Industrial Automation
- Freight
- GraphQL
- Webhook
---
