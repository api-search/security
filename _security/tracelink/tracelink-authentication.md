---
anonymous_access: false
api_key_in: []
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 4
method: searched
name: Tracelink Authentication
name_suffix: Authentication
oauth_flows: []
overview: TraceLink secures its APIs with http across 4 declared security schemes, as derived from its OpenAPI definitions.
provider_name: TraceLink
provider_slug: tracelink
scheme_count: 4
schemes:
- applies_to:
  - TraceLink Smart Event Manager REST API
  description: 'Smart Event Manager supports user-based authentication using HTTP Basic Authentication. The Base64 encoding of username:password is sent in the Authorization header alongside Content-Type: application/json.'
  name: SmartEventManagerBasic
  scheme: basic
  source: smart_event_manager_api_guide_2026.1.pdf (Getting Started with REST)
  type: http
- applies_to:
  - TraceLink OPUS Platform Event API
  - TraceLink OPUS GraphQL API
  description: 'OPUS Platform API calls authenticate with a long-lived API key and API secret pair. The two values are joined as "apiKey:apiSecret", Base64 encoded, and sent as "Authorization: Basic <encoded>". TraceLink documents the key and secret as static values that do not expire.'
  name: OpusApiKeyBasic
  scheme: basic
  source: https://github.com/tracelink/code-samples/blob/main/authentication.md
  type: http
- applies_to:
  - TraceLink OPUS Platform Event API
  description: A short-lived session token (the browser local-storage value _store_js_production_token) is used as a Bearer token for exactly one call — the authorization-manager:generate-apiKeyCredentials:v1 event — which exchanges it for the long-lived API key/secret pair. It is a bootstrap credential, not a general-purpose API token.
  name: OpusSessionBearer
  scheme: bearer
  source: https://github.com/tracelink/code-samples/blob/main/authentication.md
  type: http
- applies_to:
  - TraceLink Serialized Operations Manager (SOAP)
  - TraceLink Product Track (SOAP)
  - TraceLink Serial Number Exchange (SOAP)
  description: The SOAP services on api.tracelink.com (Serialized Operations Manager, Product Track, Serial Number Exchange) authenticate over HTTPS with HTTP Basic credentials issued by TraceLink; the guides cite RFC 7617.
  name: SoapBasic
  scheme: basic
  source: https://opus.tracelink.com/documentation/2026.1/en-US/api/som/soap/pdfs/som_soap_api_guide_2026.1.pdf
  type: http
slug: tracelink-authentication
source_filename: tracelink-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-02'\nmethod: searched\nsource: https://opus.tracelink.com/documentation/2026.1/en-US/api/smart-event-manager/pdfs/smart_event_manager_api_guide_2026.1.pdf\n  and https://github.com/tracelink/code-samples/blob/main/authentication.md\ndocs: https://github.com/tracelink/code-samples/blob/main/authentication.md\nsummary:\n  types:\n  - http\n  http_schemes:\n  - basic\n  - bearer\n  api_key_in: []\n  oauth2_flows: []\n  note: TraceLink publishes no OAuth 2.0 or OpenID Connect surface for its APIs. Every documented surface\n    authenticates with HTTP Basic (RFC 7617) or, for the short-lived bootstrap step only, a Bearer session\n    token. There is therefore no scope model and no scopes/ artifact for this provider.\nschemes:\n- name: SmartEventManagerBasic\n  type: http\n  scheme: basic\n  description: 'Smart Event Manager supports user-based authentication using HTTP Basic Authentication.\n    The Base64 encoding of username:password is sent in the Authorization\
  \ header alongside Content-Type:\n    application/json.'\n  applies_to:\n  - TraceLink Smart Event Manager REST API\n  source: smart_event_manager_api_guide_2026.1.pdf (Getting Started with REST)\n- name: OpusApiKeyBasic\n  type: http\n  scheme: basic\n  description: 'OPUS Platform API calls authenticate with a long-lived API key and API secret pair. The\n    two values are joined as \"apiKey:apiSecret\", Base64 encoded, and sent as \"Authorization: Basic <encoded>\".\n    TraceLink documents the key and secret as static values that do not expire.'\n  applies_to:\n  - TraceLink OPUS Platform Event API\n  - TraceLink OPUS GraphQL API\n  source: https://github.com/tracelink/code-samples/blob/main/authentication.md\n- name: OpusSessionBearer\n  type: http\n  scheme: bearer\n  description: A short-lived session token (the browser local-storage value _store_js_production_token)\n    is used as a Bearer token for exactly one call — the authorization-manager:generate-apiKeyCredentials:v1\n  \
  \  event — which exchanges it for the long-lived API key/secret pair. It is a bootstrap credential, not\n    a general-purpose API token.\n  applies_to:\n  - TraceLink OPUS Platform Event API\n  source: https://github.com/tracelink/code-samples/blob/main/authentication.md\n- name: SoapBasic\n  type: http\n  scheme: basic\n  description: The SOAP services on api.tracelink.com (Serialized Operations Manager, Product Track, Serial\n    Number Exchange) authenticate over HTTPS with HTTP Basic credentials issued by TraceLink; the guides\n    cite RFC 7617.\n  applies_to:\n  - TraceLink Serialized Operations Manager (SOAP)\n  - TraceLink Product Track (SOAP)\n  - TraceLink Serial Number Exchange (SOAP)\n  source: https://opus.tracelink.com/documentation/2026.1/en-US/api/som/soap/pdfs/som_soap_api_guide_2026.1.pdf\ntenancy_context:\n  description: Beyond the credential, OPUS requests carry tenancy routing values that select the company,\n    network, and dataspace the call executes in. They are\
  \ required and are effectively part of the authorization\n    context.\n  fields:\n  - name: ownerId\n    where: request body header (events API) / companyId header (GraphQL)\n    description: The Owner company associated with the request.\n  - name: processNetworkId\n    where: request body header (events API) / processNetworkId header (GraphQL)\n    description: The network within the Owner company containing the process.\n  - name: dataspace\n    where: request body header (events API) / Dataspace header (GraphQL)\n    description: The dataspace inside the environment where the request is made (e.g. \"default\").\ndocs_additional:\n- https://opus.tracelink.com/documentation/2026.1/en-US/api/smart-event-manager/pdfs/smart_event_manager_api_guide_2026.1.pdf\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tracelink/refs/heads/main/authentication/tracelink-authentication.yml
summary_line: http · 4 schemes
tags:
- Company
- Supply Chain
- Pharmaceuticals
- Life Sciences
- Serialization
- Track and Trace
- Compliance
- Healthcare
- EPCIS
- Logistics
- B2B Integration
---
