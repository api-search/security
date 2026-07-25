---
api_key_in:
- header
api_specs:
- filename: hopper-com-analytics-api-openapi.yml
  format: yaml
  label: Hopper Analytics API
  slug: hopper-com-analytics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hopper-com/refs/heads/main/openapi/hopper-com-analytics-api-openapi.yml
- filename: hopper-com-authentication-api-openapi.yml
  format: yaml
  label: Hopper Authentication API
  slug: hopper-com-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hopper-com/refs/heads/main/openapi/hopper-com-authentication-api-openapi.yml
- filename: hopper-com-cancel-for-any-reason-cfar-api-openapi.yml
  format: yaml
  label: Hopper Cancel For Any Reason (CFAR) API
  slug: hopper-com-cancel-for-any-reason-cfar-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hopper-com/refs/heads/main/openapi/hopper-com-cancel-for-any-reason-cfar-api-openapi.yml
- filename: hopper-com-disruption-guarantee-dg-api-openapi.yml
  format: yaml
  label: Hopper Disruption Guarantee (DG) API
  slug: hopper-com-disruption-guarantee-dg-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hopper-com/refs/heads/main/openapi/hopper-com-disruption-guarantee-dg-api-openapi.yml
- filename: hopper-com-sessions-api-openapi.yml
  format: yaml
  label: Hopper Sessions API
  slug: hopper-com-sessions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hopper-com/refs/heads/main/openapi/hopper-com-sessions-api-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: derived
name: Hopper Com Authentication
name_suffix: Authentication
oauth_flows: []
overview: Hopper secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Hopper
provider_slug: hopper-com
scheme_count: 2
schemes:
- description: 'This API is authenticated with OAuth 2, Client Credentials grant.\

    Clients should use their `client_id` and `client_secret` to obtain an `access_token`.\

    The `access_token` should be included in every request, as a `Bearer` token on an `Authorization` header.\

    Note that `access_token`s eventually expire, requiring a new token to be fetched.


    see [authentication](#tag/Authentication)'
  name: PartnerAuth
  scheme: bearer
  sources:
  - openapi/hopper-airlines-openapi.yml
  type: http
- description: '# Header Parameters

    | headerName      | description                                                                                        |

    |-----------------|----------------------------------------------------------------------------------------------------|

    | `HC-Session-ID` | string <br/> **Example**: `9fd3f2f9-e5aa-4128-ace9-3c4ee37b685f`<br/>The ID of the current session |'
  in: header
  name: SessionAuth
  parameter: HC-Session-ID
  sources:
  - openapi/hopper-airlines-openapi.yml
  type: apiKey
slug: hopper-com-authentication
source_filename: hopper-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/hopper-airlines-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: PartnerAuth\n  type: http\n  scheme: bearer\n  description: |-\n    This API is authenticated with OAuth 2, Client Credentials grant.\\\n    Clients should use their `client_id` and `client_secret` to obtain an `access_token`.\\\n    The `access_token` should be included in every request, as a `Bearer` token on an `Authorization` header.\\\n    Note that `access_token`s eventually expire, requiring a new token to be fetched.\n\n    see [authentication](#tag/Authentication)\n  sources:\n  - openapi/hopper-airlines-openapi.yml\n- name: SessionAuth\n  type: apiKey\n  in: header\n  parameter: HC-Session-ID\n  description: |-\n    # Header Parameters\n    | headerName      | description                                                                                        |\n    |-----------------|----------------------------------------------------------------------------------------------------|\n\
  \    | `HC-Session-ID` | string <br/> **Example**: `9fd3f2f9-e5aa-4128-ace9-3c4ee37b685f`<br/>The ID of the current session |\n  sources:\n  - openapi/hopper-airlines-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hopper-com/refs/heads/main/authentication/hopper-com-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Travel
- Travel Fintech
- Price Prediction
- Cancel For Any Reason
- Disruption Guarantee
- Price Freeze
- Airlines
- Hotels
- Car Rental
- Vacation Rentals
- Ancillary Revenue
- B2B
- Loyalty
- Agentic AI
---
