---
api_key_in:
- header
api_specs:
- filename: influxdb-openapi.yml
  format: yaml
  label: InfluxDB Cloud API
  slug: influxdb
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/influxdb/refs/heads/main/openapi/influxdb-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: derived
name: Influxdb Authentication
name_suffix: Authentication
oauth_flows: []
overview: InfluxDB secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: InfluxDB
provider_slug: influxdb
scheme_count: 2
schemes:
- description: '### Basic authentication scheme


    Use the HTTP Basic authentication scheme for InfluxDB `/api/v2` API operations that support it:


    ### Syntax


    `Authorization: Basic [example key]`


    To construct the `BASE64_ENCODED_CREDENTIALS`, combine the username and

    the password with a colon (`USERNAME:PASSWORD`), and then encode the

    resulting string in [base64](https://developer.mozilla.org/en-US/d'
  name: BasicAuthentication
  scheme: basic
  sources:
  - openapi/influxdb-openapi.yml
  type: http
- description: 'Use the [Token authentication](#section/Authentication/TokenAuthentication)

    scheme to authenticate to the InfluxDB API.


    In your API requests, send an `Authorization` header.

    For the header value, provide the word `Token` followed by a space and an InfluxDB API token.

    The word `Token` is case-sensitive.


    ### Syntax


    `Authorization: Token INFLUX_API_TOKEN`


    ### Example


    #### Use Token authenticatio'
  in: header
  name: TokenAuthentication
  parameter: Authorization
  sources:
  - openapi/influxdb-openapi.yml
  type: apiKey
slug: influxdb-authentication
source_filename: influxdb-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/influxdb-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: BasicAuthentication\n  type: http\n  scheme: basic\n  description: |-\n    ### Basic authentication scheme\n\n    Use the HTTP Basic authentication scheme for InfluxDB `/api/v2` API operations that support it:\n\n    ### Syntax\n\n    `Authorization: Basic [example key]`\n\n    To construct the `BASE64_ENCODED_CREDENTIALS`, combine the username and\n    the password with a colon (`USERNAME:PASSWORD`), and then encode the\n    resulting string in [base64](https://developer.mozilla.org/en-US/d\n  sources:\n  - openapi/influxdb-openapi.yml\n- name: TokenAuthentication\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: |-\n    Use the [Token authentication](#section/Authentication/TokenAuthentication)\n    scheme to authenticate to the InfluxDB API.\n\n    In your API requests, send an `Authorization`\
  \ header.\n    For the header value, provide the word `Token` followed by a space and an InfluxDB API token.\n    The word `Token` is case-sensitive.\n\n    ### Syntax\n\n    `Authorization: Token INFLUX_API_TOKEN`\n\n    ### Example\n\n    #### Use Token authenticatio\n  sources:\n  - openapi/influxdb-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/influxdb/refs/heads/main/authentication/influxdb-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Database
- Time Series
- Real-Time
- Analytics
---
