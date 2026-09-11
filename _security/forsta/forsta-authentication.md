---
anonymous_access: false
api_key_in:
- header
- query
api_specs:
- filename: forsta-decipher-rest-api-openapi.yml
  format: yaml
  label: Forsta Decipher REST API
  slug: forsta
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/forsta/refs/heads/main/openapi/forsta-decipher-rest-api-openapi.yml
- filename: forsta-panel-management-integration-openapi.yml
  format: yaml
  label: Forsta Panel Management APIs
  slug: panel-management
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/forsta/refs/heads/main/openapi/forsta-panel-management-integration-openapi.yml
- filename: forsta-sample-marketplace-partner-contract-openapi.yml
  format: yaml
  label: Forsta Sample Marketplace Partner APIs
  slug: sample-marketplace
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/forsta/refs/heads/main/openapi/forsta-sample-marketplace-partner-contract-openapi.yml
auth_types:
- apiKey
- http
- oauth2
description: ''
kind: authentication
layout: security
mechanism_count: 6
method: derived
name: Forsta Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: Forsta secures its APIs with apiKey, http, and oauth2 across 7 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: Forsta
provider_slug: forsta
scheme_count: 7
schemes:
- description: 'In order to access the api, you''ll need to generate an API key. Refer to the

    instructions [here](/docs/decipher/api#section/API-Keys) to generate and

    configure an API key with the appropriate permission sets. You can generate

    as many keys as required.


    Configure each request to include your API key in the request header. For example:


    ```

    x-apikey: dp48ss3mgsaucyjtybxw728h7s4cgnwzhejtszdwhf4xpe8yh'
  in: header
  name: APIKey
  parameter: x-apikey
  sources:
  - openapi/forsta-decipher-rest-api-openapi.yml
  type: apiKey
- in: query
  name: ApiKey
  parameter: seskey
  sources:
  - openapi/forsta-panel-management-community-openapi.yml
  type: apiKey
- name: BearerAuth
  scheme: bearer
  sources:
  - openapi/forsta-panel-management-integration-openapi.yml
  - openapi/forsta-panel-management-vendor-callback-openapi.yml
  type: http
- in: query
  name: ApiKey
  parameter: sesKey
  sources:
  - openapi/forsta-panel-management-integration-openapi.yml
  type: apiKey
- description: 'Security scheme for signed payloads.

    Include a signature of the payload in the "X-KP-Webhook-Signature" header.'
  in: header
  name: signedPayloadAuth
  parameter: X-KP-Webhook-Signature
  sources:
  - openapi/forsta-panel-management-webhooks-openapi.yml
  type: apiKey
- description: See https://docs.aws.amazon.com/cognito/latest/developerguide/token-endpoint.html
  flows:
  - flow: clientCredentials
    scopes: 0
    tokenUrl: /oauth2/token/
  name: OAuth2
  sources:
  - openapi/forsta-sample-marketplace-partner-contract-openapi.yml
  - openapi/forsta-sample-marketplace-partner-setup-openapi.yml
  type: oauth2
- name: BasicAuth
  scheme: basic
  sources:
  - openapi/forsta-sample-marketplace-partner-contract-openapi.yml
  - openapi/forsta-sample-marketplace-partner-setup-openapi.yml
  type: http
slug: forsta-authentication
source_filename: forsta-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-10'\nmethod: derived\nsource: openapi/forsta-decipher-rest-api-openapi.yml, openapi/forsta-panel-management-community-openapi.yml,\n  openapi/forsta-panel-management-integration-openapi.yml, openapi/forsta-panel-management-vendor-callback-openapi.yml,\n  openapi/forsta-panel-management-webhooks-openapi.yml, openapi/forsta-sample-marketplace-partner-contract-openapi.yml,\n  openapi/forsta-sample-marketplace-partner-setup-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - http\n  - oauth2\n  api_key_in:\n  - header\n  - query\n  oauth2_flows:\n  - clientCredentials\nschemes:\n- name: APIKey\n  type: apiKey\n  in: header\n  parameter: x-apikey\n  description: |-\n    In order to access the api, you'll need to generate an API key. Refer to the\n    instructions [here](/docs/decipher/api#section/API-Keys) to generate and\n    configure an API key with the appropriate permission sets. You can generate\n    as many keys as required.\n\n    Configure each request\
  \ to include your API key in the request header. For example:\n\n    ```\n    x-apikey: dp48ss3mgsaucyjtybxw728h7s4cgnwzhejtszdwhf4xpe8yh\n  sources:\n  - openapi/forsta-decipher-rest-api-openapi.yml\n- name: ApiKey\n  type: apiKey\n  in: query\n  parameter: seskey\n  sources:\n  - openapi/forsta-panel-management-community-openapi.yml\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  sources:\n  - openapi/forsta-panel-management-integration-openapi.yml\n  - openapi/forsta-panel-management-vendor-callback-openapi.yml\n- name: ApiKey\n  type: apiKey\n  in: query\n  parameter: sesKey\n  sources:\n  - openapi/forsta-panel-management-integration-openapi.yml\n- name: signedPayloadAuth\n  type: apiKey\n  in: header\n  parameter: X-KP-Webhook-Signature\n  description: |-\n    Security scheme for signed payloads.\n    Include a signature of the payload in the \"X-KP-Webhook-Signature\" header.\n  sources:\n  - openapi/forsta-panel-management-webhooks-openapi.yml\n- name: OAuth2\n  type: oauth2\n\
  \  flows:\n  - flow: clientCredentials\n    tokenUrl: /oauth2/token/\n    scopes: 0\n  description: See https://docs.aws.amazon.com/cognito/latest/developerguide/token-endpoint.html\n  sources:\n  - openapi/forsta-sample-marketplace-partner-contract-openapi.yml\n  - openapi/forsta-sample-marketplace-partner-setup-openapi.yml\n- name: BasicAuth\n  type: http\n  scheme: basic\n  sources:\n  - openapi/forsta-sample-marketplace-partner-contract-openapi.yml\n  - openapi/forsta-sample-marketplace-partner-setup-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/forsta/refs/heads/main/authentication/forsta-authentication.yml
summary_line: apiKey/http/oauth2 · 7 schemes
tags:
- Customer Insights
- Feedback
- Market Research
- Surveys
- Customer Experience
- Employee Experience
- Panel Management
- Data Collection
- Analytics
- Voice of the Customer
---
