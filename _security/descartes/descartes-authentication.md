---
anonymous_access: false
api_key_in: []
api_specs:
- filename: descartes-3rd-party-tms-integration-api-openapi.yml
  format: yaml
  label: Descartes Systems Group 3rd Party TMS Integration API
  slug: descartes-3rd-party-tms-integration-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/descartes/refs/heads/main/openapi/descartes-3rd-party-tms-integration-api-openapi.yml
- filename: descartes-api-xml-api-openapi.yml
  format: yaml
  label: Descartes Systems Group API - XML API
  slug: descartes-api-xml-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/descartes/refs/heads/main/openapi/descartes-api-xml-api-openapi.yml
- filename: descartes-carrier-data-connection-and-communication-api-openapi.yml
  format: yaml
  label: Descartes Systems Group Carrier Data Connection and Communication API
  slug: descartes-carrier-data-connection-and-communication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/descartes/refs/heads/main/openapi/descartes-carrier-data-connection-and-communication-api-openapi.yml
- filename: descartes-custom-integration-api-openapi.yml
  format: yaml
  label: Descartes Systems Group Custom Integration API
  slug: descartes-custom-integration-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/descartes/refs/heads/main/openapi/descartes-custom-integration-api-openapi.yml
- filename: descartes-export-api-api-openapi.yml
  format: yaml
  label: Descartes Systems Group Export API
  slug: descartes-export-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/descartes/refs/heads/main/openapi/descartes-export-api-api-openapi.yml
- filename: descartes-fraudguard-carrier-and-load-lookup-api-openapi.yml
  format: yaml
  label: Descartes Systems Group FraudGuard Carrier and Load Lookup API
  slug: descartes-fraudguard-carrier-and-load-lookup-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/descartes/refs/heads/main/openapi/descartes-fraudguard-carrier-and-load-lookup-api-openapi.yml
- filename: descartes-import-api-api-openapi.yml
  format: yaml
  label: Descartes Systems Group Import API
  slug: descartes-import-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/descartes/refs/heads/main/openapi/descartes-import-api-api-openapi.yml
- filename: descartes-load-visibility-order-creation-xml-api-openapi.yml
  format: yaml
  label: Descartes Systems Group Load Visibility Order Creation - XML API
  slug: descartes-load-visibility-order-creation-xml-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/descartes/refs/heads/main/openapi/descartes-load-visibility-order-creation-xml-api-openapi.yml
- filename: descartes-load-visibility-url-and-data-export-retrieval-api-openapi.yml
  format: yaml
  label: Descartes Systems Group Load Visibility URL and Data Export Retrieval API
  slug: descartes-load-visibility-url-and-data-export-retrieval-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/descartes/refs/heads/main/openapi/descartes-load-visibility-url-and-data-export-retrieval-api-openapi.yml
- filename: descartes-search-api-api-openapi.yml
  format: yaml
  label: Descartes Systems Group Search API
  slug: descartes-search-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/descartes/refs/heads/main/openapi/descartes-search-api-api-openapi.yml
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Descartes Authentication
name_suffix: Authentication
oauth_flows: []
overview: Descartes Systems Group declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Descartes Systems Group
provider_slug: descartes
scheme_count: 2
schemes:
- applies_to: Customer to Descartes MacroPoint APIs (macropoint-lite.com/api/1.0) and carrier integration APIs
  evidence: 'API Base Configuration — Base URL: https://macropoint-lite.com/api/1.0/ Authentication: Basic'
  name: basicAuth
  scheme: basic
  type: http
- direction: outbound (Descartes MacroPoint to customer webhook callbacks)
  evidence: 'Authentication: Basic or Oauth. Oauth requires a token URL, Client ID, Client Secret, Grant Type, and optional Scope'
  name: callbackAuth
  type: http-or-oauth2
slug: descartes-authentication
source_filename: descartes-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "name: Descartes MacroPoint authentication\ngenerated: '2026-10-20'\nmethod: searched\nsource: https://docs.macropoint.com/\ndocs: https://docs.macropoint.com/\nschemes:\n- name: basicAuth\n  type: http\n  scheme: basic\n  applies_to: Customer to Descartes MacroPoint APIs (macropoint-lite.com/api/1.0) and carrier integration APIs\n  evidence: \"API Base Configuration — Base URL: https://macropoint-lite.com/api/1.0/ Authentication: Basic\"\n- name: callbackAuth\n  type: http-or-oauth2\n  direction: outbound (Descartes MacroPoint to customer webhook callbacks)\n  evidence: \"Authentication: Basic or Oauth. Oauth requires a token URL, Client ID, Client Secret, Grant Type, and optional Scope\"\nnote: Credentials are issued to MacroPoint customers and carriers; there is no self-service key signup.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/descartes/refs/heads/main/authentication/descartes-authentication.yml
summary_line: 2 schemes
tags:
- Logistics
- Supply Chain
- Freight Visibility
- Shipment Tracking
- Customs Compliance
- Global Trade
- Trade Content
- Carrier Sourcing
---
