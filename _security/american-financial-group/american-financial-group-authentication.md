---
api_key_in: []
api_specs:
- filename: american-financial-group-shop-openapi.yml
  format: yaml
  label: Great American Carrier Services Shop API
  slug: great-american-carrier-services-shop-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/american-financial-group/refs/heads/main/openapi/american-financial-group-shop-openapi.yml
- filename: american-financial-group-submission-openapi.yml
  format: yaml
  label: Great American Carrier Services Submission API
  slug: great-american-carrier-services-submission-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/american-financial-group/refs/heads/main/openapi/american-financial-group-submission-openapi.yml
- filename: american-financial-group-product-openapi.yml
  format: yaml
  label: Great American Carrier Services Product API
  slug: great-american-carrier-services-product-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/american-financial-group/refs/heads/main/openapi/american-financial-group-product-openapi.yml
- filename: american-financial-group-risk-selection-openapi.yml
  format: yaml
  label: Great American Carrier Services Risk Selection API
  slug: great-american-carrier-services-risk-selection-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/american-financial-group/refs/heads/main/openapi/american-financial-group-risk-selection-openapi.yml
- filename: american-financial-group-rating-openapi.yml
  format: yaml
  label: Great American Carrier Services Rating API
  slug: great-american-carrier-services-rating-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/american-financial-group/refs/heads/main/openapi/american-financial-group-rating-openapi.yml
- filename: american-financial-group-forms-openapi.yml
  format: yaml
  label: Great American Carrier Services Forms API
  slug: great-american-carrier-services-forms-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/american-financial-group/refs/heads/main/openapi/american-financial-group-forms-openapi.yml
- filename: american-financial-group-issuance-openapi.yml
  format: yaml
  label: Great American Carrier Services Issuance API
  slug: great-american-carrier-services-issuance-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/american-financial-group/refs/heads/main/openapi/american-financial-group-issuance-openapi.yml
- filename: american-financial-group-policy-openapi.yml
  format: yaml
  label: Great American Carrier Services Policy API
  slug: great-american-carrier-services-policy-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/american-financial-group/refs/heads/main/openapi/american-financial-group-policy-openapi.yml
- filename: american-financial-group-document-openapi.yml
  format: yaml
  label: Great American Carrier Services Document API
  slug: great-american-carrier-services-document-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/american-financial-group/refs/heads/main/openapi/american-financial-group-document-openapi.yml
- filename: american-financial-group-billing-openapi.yml
  format: yaml
  label: Great American Carrier Services Billing API
  slug: great-american-carrier-services-billing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/american-financial-group/refs/heads/main/openapi/american-financial-group-billing-openapi.yml
- filename: american-financial-group-ingestion-openapi.yml
  format: yaml
  label: Great American Carrier Services Ingestion API
  slug: great-american-carrier-services-ingestion-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/american-financial-group/refs/heads/main/openapi/american-financial-group-ingestion-openapi.yml
- filename: american-financial-group-risk-assessment-openapi.yml
  format: yaml
  label: Great American Carrier Services Risk Assessment API
  slug: great-american-carrier-services-risk-assessment-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/american-financial-group/refs/heads/main/openapi/american-financial-group-risk-assessment-openapi.yml
- filename: american-financial-group-letters-openapi.yml
  format: yaml
  label: Great American Carrier Services Letters API
  slug: great-american-carrier-services-letters-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/american-financial-group/refs/heads/main/openapi/american-financial-group-letters-openapi.yml
- filename: american-financial-group-producer-openapi.yml
  format: yaml
  label: Great American Carrier Services Producer API
  slug: great-american-carrier-services-producer-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/american-financial-group/refs/heads/main/openapi/american-financial-group-producer-openapi.yml
- filename: american-financial-group-contract-openapi.yml
  format: yaml
  label: Great American Carrier Services Contract API
  slug: great-american-carrier-services-contract-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/american-financial-group/refs/heads/main/openapi/american-financial-group-contract-openapi.yml
- filename: american-financial-group-opportunity-openapi.yml
  format: yaml
  label: Great American Carrier Services Opportunity API
  slug: great-american-carrier-services-opportunity-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/american-financial-group/refs/heads/main/openapi/american-financial-group-opportunity-openapi.yml
- filename: american-financial-group-notification-openapi.yml
  format: yaml
  label: Great American Carrier Services Notification API
  slug: great-american-carrier-services-notification-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/american-financial-group/refs/heads/main/openapi/american-financial-group-notification-openapi.yml
- filename: american-financial-group-claims-openapi.yml
  format: yaml
  label: Great American Carrier Services Claims API
  slug: great-american-carrier-services-claims-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/american-financial-group/refs/heads/main/openapi/american-financial-group-claims-openapi.yml
auth_types: []
description: ''
kind: authentication
layout: security
method: searched
name: American Financial Group Authentication
name_suffix: Authentication
oauth_flows: []
overview: American Financial Group declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: American Financial Group
provider_slug: american-financial-group
scheme_count: 1
schemes:
- applies_to: all endpoints on all 18 published APIs
  client_authentication: http_basic
  exceptions:
  - api: ingestion
    endpoint: POST /api/webhook/{name}
    note: Documented as an unauthenticated endpoint designed for inbound webhooks. It only works for known, pre-configured webhook names and the request is verified in a custom manner per name.
  flow: clientCredentials
  header: Authorization
  id: oauth2_client_credentials
  in: header
  scheme: Bearer
  token_endpoints:
    dev: https://dev01.api.gaig.com/oauth/token
    prod: https://prod01.api.gaig.com/oauth/token
    uat: https://uat01.api.gaig.com/oauth/token
  token_request:
    body: grant_type=client_credentials
    content_type: application/x-www-form-urlencoded
    method: POST
    path: /oauth/token
  token_response_fields:
  - description: Bearer token to place in the Authorization header.
    name: access_token
  - description: Always Bearer; prefixes the access_token in the Authorization header.
    name: token_type
  - description: Token lifetime in seconds. Documented example value is 3599.
    name: expires_in
  - description: Array of strings naming the API products (authorities) granted to this client, e.g. ["issuance-dev","rating-dev"]. This is the authorization surface in place of named OAuth scopes.
    name: api_product_list_json
  type: oauth2
slug: american-financial-group-authentication
source_filename: american-financial-group-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-02'\nmethod: searched\nsource: https://api-documentation.gaig.com/policy/index.html\ndocs: https://api-documentation.gaig.com/policy/index.html\nsummary: >-\n  Every endpoint on every Great American Carrier Services API is secured with OAuth 2.0 using the\n  client_credentials grant. The client authenticates to the environment token endpoint with HTTP Basic\n  (base64 clientId:clientSecret), receives a bearer access token valid for 3599 seconds, and presents it\n  as `Authorization: Bearer {access_token}` on API calls. Credentials are issued by Great American through\n  the Carrier Services onboarding engagement — there is no self-service key issuance.\nschemes:\n  - id: oauth2_client_credentials\n    type: oauth2\n    flow: clientCredentials\n    in: header\n    header: Authorization\n    scheme: Bearer\n    client_authentication: http_basic\n    token_request:\n      method: POST\n      path: /oauth/token\n      content_type: application/x-www-form-urlencoded\n\
  \      body: grant_type=client_credentials\n    token_endpoints:\n      dev: https://dev01.api.gaig.com/oauth/token\n      uat: https://uat01.api.gaig.com/oauth/token\n      prod: https://prod01.api.gaig.com/oauth/token\n    token_response_fields:\n      - name: access_token\n        description: Bearer token to place in the Authorization header.\n      - name: token_type\n        description: Always Bearer; prefixes the access_token in the Authorization header.\n      - name: expires_in\n        description: Token lifetime in seconds. Documented example value is 3599.\n      - name: api_product_list_json\n        description: >-\n          Array of strings naming the API products (authorities) granted to this client, e.g.\n          [\"issuance-dev\",\"rating-dev\"]. This is the authorization surface in place of named OAuth scopes.\n    applies_to: all endpoints on all 18 published APIs\n    exceptions:\n      - endpoint: POST /api/webhook/{name}\n        api: ingestion\n        note:\
  \ >-\n          Documented as an unauthenticated endpoint designed for inbound webhooks. It only works for\n          known, pre-configured webhook names and the request is verified in a custom manner per name.\ngateway:\n  vendor_signal: Apigee\n  evidence: >-\n    401 responses are documented with the Apigee fault envelope\n    {\"fault\":{\"faultstring\":\"Invalid Access Token\",\"detail\":{\"errorcode\":\"keymanagement.service.invalid_access_token\"}}}\nnetwork_controls:\n  ip_allowlist: true\n  evidence:\n    url: https://prod01.api.gaig.com/oauth/token\n    status: 500\n    body: 'Access Denied for client ip : [<probe-ip>]'\n    note: >-\n      An anonymous POST to the production token endpoint is rejected at the network layer before any\n      credential check, which means consumer source IPs are allowlisted as part of onboarding.\nmtls: false\napi_keys: false\nopenid_connect: false\nuser_delegated_auth: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/american-financial-group/refs/heads/main/authentication/american-financial-group-authentication.yml
summary_line: 1 scheme
tags:
- Insurance
- Property Casualty
- Specialty Insurance
- Annuities
- Financial-Services
- Commercial Insurance
- Fortune 500
---
