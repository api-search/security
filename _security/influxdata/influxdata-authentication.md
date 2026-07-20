---
api_key_in:
- header
api_specs:
- filename: influxdata-cloud-openapi-original.yml
  format: yaml
  label: InfluxDB Cloud API
  slug: influxdb-cloud-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/influxdata/refs/heads/main/openapi/influxdata-cloud-openapi-original.yml
- filename: influxdata-oss-openapi-original.yml
  format: yaml
  label: InfluxDB OSS API
  slug: influxdb-oss-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/influxdata/refs/heads/main/openapi/influxdata-oss-openapi-original.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: derived
name: Influxdata Authentication
name_suffix: Authentication
oauth_flows: []
overview: InfluxData secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: InfluxData
provider_slug: influxdata
scheme_count: 2
schemes:
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
  - openapi/influxdata-cloud-openapi-original.yml
  - openapi/influxdata-oss-openapi-original.yml
  type: apiKey
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
  - openapi/influxdata-cloud-openapi-original.yml
  - openapi/influxdata-oss-openapi-original.yml
  type: http
slug: influxdata-authentication
source_filename: influxdata-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: derived\nsource: openapi/influxdata-cloud-openapi-original.yml, openapi/influxdata-oss-openapi-original.yml\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: TokenAuthentication\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: |-\n    Use the [Token authentication](#section/Authentication/TokenAuthentication)\n    scheme to authenticate to the InfluxDB API.\n\n    In your API requests, send an `Authorization` header.\n    For the header value, provide the word `Token` followed by a space and an InfluxDB API token.\n    The word `Token` is case-sensitive.\n\n    ### Syntax\n\n    `Authorization: Token INFLUX_API_TOKEN`\n\n    ### Example\n\n    #### Use Token authenticatio\n  sources:\n  - openapi/influxdata-cloud-openapi-original.yml\n  - openapi/influxdata-oss-openapi-original.yml\n- name: BasicAuthentication\n  type: http\n  scheme: basic\n  description: |-\n    ### Basic authentication\
  \ scheme\n\n    Use the HTTP Basic authentication scheme for InfluxDB `/api/v2` API operations that support it:\n\n    ### Syntax\n\n    `Authorization: Basic [example key]`\n\n    To construct the `BASE64_ENCODED_CREDENTIALS`, combine the username and\n    the password with a colon (`USERNAME:PASSWORD`), and then encode the\n    resulting string in [base64](https://developer.mozilla.org/en-US/d\n  sources:\n  - openapi/influxdata-cloud-openapi-original.yml\n  - openapi/influxdata-oss-openapi-original.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/influxdata/refs/heads/main/authentication/influxdata-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Time Series Database
- Database
- Monitoring
- Observability
- IoT
- Metrics
- Analytics
- DevOps
- Real-Time Data
- InfluxDB
- Telegraf
- Company
---
