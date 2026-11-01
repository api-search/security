---
anonymous_access: false
api_key_in: []
api_specs:
- filename: evergreen-marine-an-publisher-endpoints-api-openapi.yml
  format: yaml
  label: Evergreen Marine Corp. AN Publisher Endpoints API
  slug: evergreen-marine-an-publisher-endpoints-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/evergreen-marine/openapi/evergreen-marine-an-publisher-endpoints-api-openapi.yml
- filename: evergreen-marine-an-subscriber-endpoints-api-openapi.yml
  format: yaml
  label: Evergreen Marine Corp. AN Subscriber Endpoints API
  slug: evergreen-marine-an-subscriber-endpoints-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/evergreen-marine/openapi/evergreen-marine-an-subscriber-endpoints-api-openapi.yml
- filename: evergreen-marine-booking-api-openapi.yml
  format: yaml
  label: Evergreen Marine Corp. Booking API
  slug: evergreen-marine-booking-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/evergreen-marine/openapi/evergreen-marine-booking-api-openapi.yml
- filename: evergreen-marine-events-api-openapi.yml
  format: yaml
  label: Evergreen Marine Corp. Events API
  slug: evergreen-marine-events-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/evergreen-marine/openapi/evergreen-marine-events-api-openapi.yml
- filename: evergreen-marine-issuance-response-api-openapi.yml
  format: yaml
  label: Evergreen Marine Corp. Issuance Response API
  slug: evergreen-marine-issuance-response-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/evergreen-marine/openapi/evergreen-marine-issuance-response-api-openapi.yml
- filename: evergreen-marine-notifications-api-openapi.yml
  format: yaml
  label: Evergreen Marine Corp. Notifications API
  slug: evergreen-marine-notifications-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/evergreen-marine/openapi/evergreen-marine-notifications-api-openapi.yml
- filename: evergreen-marine-point-to-point-api-openapi.yml
  format: yaml
  label: Evergreen Marine Corp. Point To Point API
  slug: evergreen-marine-point-to-point-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/evergreen-marine/openapi/evergreen-marine-point-to-point-api-openapi.yml
- filename: evergreen-marine-port-schedule-api-openapi.yml
  format: yaml
  label: Evergreen Marine Corp. Port Schedule API
  slug: evergreen-marine-port-schedule-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/evergreen-marine/openapi/evergreen-marine-port-schedule-api-openapi.yml
- filename: evergreen-marine-shipping-instructions-api-openapi.yml
  format: yaml
  label: Evergreen Marine Corp. Shipping Instructions API
  slug: evergreen-marine-shipping-instructions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/evergreen-marine/openapi/evergreen-marine-shipping-instructions-api-openapi.yml
- filename: evergreen-marine-subscriptions-api-openapi.yml
  format: yaml
  label: Evergreen Marine Corp. Subscriptions API
  slug: evergreen-marine-subscriptions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/evergreen-marine/openapi/evergreen-marine-subscriptions-api-openapi.yml
- filename: evergreen-marine-surrender-requests-api-openapi.yml
  format: yaml
  label: Evergreen Marine Corp. Surrender Requests API
  slug: evergreen-marine-surrender-requests-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/evergreen-marine/openapi/evergreen-marine-surrender-requests-api-openapi.yml
- filename: evergreen-marine-transport-document-api-openapi.yml
  format: yaml
  label: Evergreen Marine Corp. Transport Document API
  slug: evergreen-marine-transport-document-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/evergreen-marine/openapi/evergreen-marine-transport-document-api-openapi.yml
- filename: evergreen-marine-vessel-schedule-api-openapi.yml
  format: yaml
  label: Evergreen Marine Corp. Vessel Schedule API
  slug: evergreen-marine-vessel-schedule-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/evergreen-marine/openapi/evergreen-marine-vessel-schedule-api-openapi.yml
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Evergreen Marine Authentication
name_suffix: Authentication
oauth_flows: []
overview: Evergreen Marine Corp. declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Evergreen Marine Corp.
provider_slug: evergreen-marine
scheme_count: 2
schemes:
- description: JWT token obtained using Client ID and secret provided after registration
  evidence: 'FAQ Question 3: "How do I get JWT for API Service?"

    Answer: "After your registration, you may receive a confirmation letter with Client ID & secret get token (JWT) for the pull/push API service. By using Client ID & secret with your request body (header/payload) to ask our JWT Service. After check, Evergreen will return you a token with JWT format ( https://jwt.io ). Using JWT token embed in your client application to call API service. Evergreen will decrypt token and verify payload, to make sure API request is from right party and valid."

    '
  flow: clientCredentials
  name: JWT Authentication
  notes: 'After registration, customers receive a confirmation letter with Client ID & secret to get token (JWT) for the pull/push API service.

    Using Client ID & secret with request body (header/payload) to ask our JWT Service.

    Evergreen returns a token with JWT format (https://jwt.io).

    Using JWT token embedded in client application to call API service.

    Evergreen decrypts token and verifies payload to ensure API request is from right party and valid.

    '
  scopes: []
  tokenUrl: Provided after registration (JWT Service)
  type: oauth2
- description: API-Version header MUST be added to requests
  evidence: Found in OpenAPI specifications
  in: header
  keyName: API-Version
  name: API-Version Header
  notes: API-Version header MAY be added to the request (optional); if added it MUST only contain MAJOR version. API-Version header MUST be aligned with the URI version.
  type: apiKey
slug: evergreen-marine-authentication
source_filename: evergreen-marine-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-18'\nmethod: searched\nsource: https://www.shipmentlink.com/_ec/APIPORTAL_FAQ\ndocs: https://www.shipmentlink.com/_ec/APIPORTAL_FAQ\nschemes:\n- type: oauth2\n  name: JWT Authentication\n  description: JWT token obtained using Client ID and secret provided after registration\n  flow: clientCredentials\n  tokenUrl: Provided after registration (JWT Service)\n  scopes: []\n  notes: |\n    After registration, customers receive a confirmation letter with Client ID & secret to get token (JWT) for the pull/push API service.\n    Using Client ID & secret with request body (header/payload) to ask our JWT Service.\n    Evergreen returns a token with JWT format (https://jwt.io).\n    Using JWT token embedded in client application to call API service.\n    Evergreen decrypts token and verifies payload to ensure API request is from right party and valid.\n  evidence: |\n    FAQ Question 3: \"How do I get JWT for API Service?\"\n    Answer: \"After your registration,\
  \ you may receive a confirmation letter with Client ID & secret get token (JWT) for the pull/push API service. By using Client ID & secret with your request body (header/payload) to ask our JWT Service. After check, Evergreen will return you a token with JWT format ( https://jwt.io ). Using JWT token embed in your client application to call API service. Evergreen will decrypt token and verify payload, to make sure API request is from right party and valid.\"\n- type: apiKey\n  name: API-Version Header\n  description: API-Version header MUST be added to requests\n  in: header\n  keyName: API-Version\n  notes: API-Version header MAY be added to the request (optional); if added it MUST only contain MAJOR version. API-Version header MUST be aligned with the URI version.\n  evidence: Found in OpenAPI specifications"
source_yaml_url: https://artifacts.apis.io/evergreen-marine/authentication/evergreen-marine-authentication.yml
summary_line: 2 schemes
tags:
- Company
- Container Shipping
- Logistics
- Maritime
- Shipping
- Supply Chain
- Track and Trace
- Taiwan
---
