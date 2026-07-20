---
api_key_in:
- header
api_specs:
- filename: despegar-hotels-openapi.json
  format: json
  label: Despegar Hotels API
  slug: despegar-hotels-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/despegar/refs/heads/main/openapi/despegar-hotels-openapi.json
- filename: despegar-flights-openapi.json
  format: json
  label: Despegar Flights API
  slug: despegar-flights-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/despegar/refs/heads/main/openapi/despegar-flights-openapi.json
- filename: despegar-activities-openapi.json
  format: json
  label: Despegar Activities API
  slug: despegar-activities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/despegar/refs/heads/main/openapi/despegar-activities-openapi.json
- filename: despegar-booking-openapi.json
  format: json
  label: Despegar Booking API
  slug: despegar-booking-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/despegar/refs/heads/main/openapi/despegar-booking-openapi.json
- filename: despegar-aftersales-openapi.json
  format: json
  label: Despegar Aftersales API
  slug: despegar-aftersales-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/despegar/refs/heads/main/openapi/despegar-aftersales-openapi.json
- filename: despegar-geo-openapi.json
  format: json
  label: Despegar Common Assets API
  slug: despegar-common-assets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/despegar/refs/heads/main/openapi/despegar-geo-openapi.json
auth_types:
- apiKey
- http
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Despegar Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: Despegar secures its APIs with apiKey, http, and oauth2 across 3 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: Despegar
provider_slug: despegar
scheme_count: 3
schemes:
- description: Primary B2B credential; provisioned per client at onboarding, distinct test vs production keys.
  in: header
  name: ApiKeyAuth
  parameter: x-apikey
  sources:
  - openapi/despegar-booking-openapi.json
  - openapi/despegar-hotels-openapi.json
  - openapi/despegar-flights-openapi.json
  - openapi/despegar-aftersales-openapi.json
  - openapi/despegar-activities-openapi.json
  - openapi/despegar-geo-openapi.json
  type: apiKey
- bearerFormat: JWT
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/despegar-booking-openapi.json
  - openapi/despegar-hotels-openapi.json
  - openapi/despegar-flights-openapi.json
  - openapi/despegar-aftersales-openapi.json
  - openapi/despegar-activities-openapi.json
  - openapi/despegar-geo-openapi.json
  type: http
- description: OAuth 2.0 client_credentials used by the Despegar MCP B2B flights/hotels servers; credentials handled server-side.
  flow: clientCredentials
  name: MCP OAuth2
  sources:
  - https://api-docs.despegar.com/docs/mcp-support
  type: oauth2
slug: despegar-authentication
source_filename: despegar-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: openapi/despegar-booking-openapi.json (+ hotels/flights/aftersales/activities/geo)\ndocs: https://api-docs.despegar.com/docs/security-scheme\nnotes: >-\n  The B2B Despegar REST API is authenticated with a single API key sent in the\n  x-apikey header. Keys are provisioned per client during onboarding with\n  permissions tailored to the products contracted, and separate keys exist for\n  the test and production environments. A JWT bearer scheme (BearerAuth) is also\n  declared in the OpenAPI. The separately documented MCP B2B servers use OAuth\n  2.0 client_credentials (see mcp/despegar-mcp.yml).\nsummary:\n  types:\n  - apiKey\n  - http\n  - oauth2\n  api_key_in:\n  - header\n  oauth2_flows:\n  - clientCredentials\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: x-apikey\n  description: Primary B2B credential; provisioned per client at onboarding, distinct test vs production keys.\n  sources:\n  - openapi/despegar-booking-openapi.json\n\
  \  - openapi/despegar-hotels-openapi.json\n  - openapi/despegar-flights-openapi.json\n  - openapi/despegar-aftersales-openapi.json\n  - openapi/despegar-activities-openapi.json\n  - openapi/despegar-geo-openapi.json\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  sources:\n  - openapi/despegar-booking-openapi.json\n  - openapi/despegar-hotels-openapi.json\n  - openapi/despegar-flights-openapi.json\n  - openapi/despegar-aftersales-openapi.json\n  - openapi/despegar-activities-openapi.json\n  - openapi/despegar-geo-openapi.json\n- name: MCP OAuth2\n  type: oauth2\n  flow: clientCredentials\n  description: OAuth 2.0 client_credentials used by the Despegar MCP B2B flights/hotels servers; credentials handled server-side.\n  sources:\n  - https://api-docs.despegar.com/docs/mcp-support\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/despegar/refs/heads/main/authentication/despegar-authentication.yml
summary_line: apiKey/http/oauth2 · 3 schemes
tags:
- Company
- Consumer
- Travel
- Hotels
- Flights
- Booking
- Tourism
- Latin America
- B2B
- MCP
---
