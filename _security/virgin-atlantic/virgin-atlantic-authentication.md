---
api_key_in:
- header
auth_types:
- apiKey
description: Virgin Atlantic's NDC API authenticates with a single API key carried in an HTTP header. There is no OAuth 2.0, no OpenID Connect, no mTLS and no signed-request scheme published anywhere on VS NDC Connect, and no OpenAPI exists from which securitySchemes could be derived - this profile is read directly from the published build documentation. The header name and the Azure Front Door DNS for ndc.virginatlantic.com indicate the gateway is Microsoft Azure API Management.
kind: authentication
layout: security
method: searched
name: Virgin Atlantic Authentication
name_suffix: Authentication
oauth_flows: []
overview: Virgin Atlantic secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Virgin Atlantic
provider_slug: virgin-atlantic
scheme_count: 1
schemes:
- environments:
  - Test
  - Production
  example_header: 'Ocp-Apim-Subscription-Key: [API-KEY-VALUE]'
  failure_code: 111 - Invalid Agent's IATA API Key
  gateway: Microsoft Azure API Management (inferred from the Ocp-Apim-Subscription-Key header name and the avahfrontdoorprod.azurefd.net Azure Front Door DNS)
  in: header
  name: VSNDCApiKey
  parameter_name: Ocp-Apim-Subscription-Key
  sources:
  - https://ndc.virginatlantic.com/help/how-to-start-your-build
  type: apiKey
  verbatim: '"The HTTP header must include your API Client Key to grant access to the API. This would have been provided to you as part of the NDC API Access process."'
slug: virgin-atlantic-authentication
source_filename: virgin-atlantic-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-28'\nmethod: searched\nsource: >-\n  https://ndc.virginatlantic.com/help/how-to-start-your-build,\n  https://ndc.virginatlantic.com/help/how-to-access-ndc-apis,\n  https://ndc.virginatlantic.com/certification,\n  https://ndc.virginatlantic.com/docs/orderchangenotif\ndocs: https://ndc.virginatlantic.com/help/how-to-start-your-build\ndescription: >-\n  Virgin Atlantic's NDC API authenticates with a single API key carried in an HTTP header. There is\n  no OAuth 2.0, no OpenID Connect, no mTLS and no signed-request scheme published anywhere on VS NDC\n  Connect, and no OpenAPI exists from which securitySchemes could be derived - this profile is read\n  directly from the published build documentation. The header name and the Azure Front Door DNS for\n  ndc.virginatlantic.com indicate the gateway is Microsoft Azure API Management.\nsummary:\n  types: [apiKey]\n  api_key_in: [header]\n  oauth2_flows: []\n  oidc: false\n  mutual_tls: false\nschemes:\n  - name: VSNDCApiKey\n\
  \    type: apiKey\n    in: header\n    parameter_name: Ocp-Apim-Subscription-Key\n    example_header: 'Ocp-Apim-Subscription-Key: [API-KEY-VALUE]'\n    verbatim: >-\n      \"The HTTP header must include your API Client Key to grant access to the API. This would have\n      been provided to you as part of the NDC API Access process.\"\n    gateway: Microsoft Azure API Management (inferred from the Ocp-Apim-Subscription-Key header name\n      and the avahfrontdoorprod.azurefd.net Azure Front Door DNS)\n    environments: [Test, Production]\n    failure_code: '111 - Invalid Agent''s IATA API Key'\n    sources: [https://ndc.virginatlantic.com/help/how-to-start-your-build]\nrequest_headers:\n  - {name: Ocp-Apim-Subscription-Key, value: '[API-KEY-VALUE]', required: true, note: VS NDC API key}\n  - {name: Accept, value: application/xml, required: true}\n  - {name: Content-Type, value: application/xml, required: true}\nencoding: UTF-8 required on both request and response\ntransport:\n  method:\
  \ POST\n  note: >-\n    \"We make a POST call to all of our API endpoints\" - every NDC message is an HTTP POST with an\n    IATA NDC 21.3 XML body. No base URL is published; endpoints are issued with the key.\ncallback_authentication:\n  surface: OrderChangeNotif (airline-to-seller push)\n  note: >-\n    Registering to receive OrderChangeNotif requires the seller to supply its own endpoint URL, SOAP\n    Action and API login credentials (UserID and Password) plus API username/key and IATA number /\n    Aggregator ID - so the inbound direction is authenticated by seller-supplied credentials, not by\n    a Virgin Atlantic signature header.\n  docs: https://ndc.virginatlantic.com/docs/orderchangenotif\n  detail: asyncapi/virgin-atlantic-orderchangenotif-webhooks.yml\naccess_gate:\n  self_serve_test_key: true\n  production_requirements:\n    - Valid IATA accreditation and Virgin Atlantic ticketing authority (Direct Connection), or an\n      approved Service Provider Connection\n    - RED\
  \ Tier certification minimum\n    - Signed Technical User Agreement (TUA), Data Processing Agreement (DPA) and, for agents, the\n      Agency Sales Agreement (ASA)\n  docs: https://ndc.virginatlantic.com/help/how-to-access-ndc-apis\nnot_published:\n  - OAuth 2.0 / OpenID Connect (no /.well-known/openid-configuration or oauth-authorization-server\n    document exists on any Virgin Atlantic host - see well-known/virgin-atlantic-well-known.yml)\n  - Scopes or permission model (no OAuth surface, so scopes/ is intentionally absent)\n  - Key rotation policy, key expiry or per-key rate limits\n  - Request signing, mTLS or IP allow-listing requirements\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/virgin-atlantic/refs/heads/main/authentication/virgin-atlantic-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Travel
- United Kingdom
- Aviation
- Airline
- Distribution
- NDC
- Booking
- GDS
---
