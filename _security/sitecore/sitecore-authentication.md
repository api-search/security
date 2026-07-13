---
api_key_in:
- header
api_specs:
- filename: sitecore-xm-cloud-rest-api-openapi.yml
  format: yaml
  label: Sitecore XM Cloud REST API
  slug: xm-cloud-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sitecore/refs/heads/main/openapi/sitecore-xm-cloud-rest-api-openapi.yml
- filename: sitecore-cdp-rest-api-openapi.yml
  format: yaml
  label: Sitecore CDP REST API
  slug: cdp-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sitecore/refs/heads/main/openapi/sitecore-cdp-rest-api-openapi.yml
- filename: sitecore-cdp-stream-api-asyncapi.yml
  format: yaml
  label: Sitecore CDP Stream API
  slug: cdp-stream-api
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/sitecore/refs/heads/main/asyncapi/sitecore-cdp-stream-api-asyncapi.yml
- filename: sitecore-personalize-rest-api-openapi.yml
  format: yaml
  label: Sitecore Personalize REST API
  slug: personalize-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sitecore/refs/heads/main/openapi/sitecore-personalize-rest-api-openapi.yml
- filename: sitecore-content-hub-rest-api-openapi.yml
  format: yaml
  label: Sitecore Content Hub REST API
  slug: content-hub-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sitecore/refs/heads/main/openapi/sitecore-content-hub-rest-api-openapi.yml
- filename: sitecore-ordercloud-api-openapi.yml
  format: yaml
  label: Sitecore OrderCloud API
  slug: ordercloud-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sitecore/refs/heads/main/openapi/sitecore-ordercloud-api-openapi.yml
- filename: sitecore-discover-api-openapi.yml
  format: yaml
  label: Sitecore Discover API
  slug: discover-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sitecore/refs/heads/main/openapi/sitecore-discover-api-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: derived
name: Sitecore Authentication
name_suffix: Authentication
oauth_flows: []
overview: sitecore secures its APIs with apiKey and http across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: sitecore
provider_slug: sitecore
scheme_count: 3
schemes:
- description: HTTP Basic authentication using a client key as the username and an API token as the password. Credentials are obtained from Sitecore CDP Settings > API access.
  name: basicAuth
  scheme: basic
  sources:
  - openapi/sitecore-cdp-rest-api-openapi.yml
  type: http
- bearerFormat: JWT
  description: OAuth 2.0 bearer token obtained from the Content Hub identity provider. Include the token in the Authorization header as 'Bearer {token}'.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/sitecore-content-hub-rest-api-openapi.yml
  - openapi/sitecore-discover-api-openapi.yml
  - openapi/sitecore-ordercloud-api-openapi.yml
  - openapi/sitecore-xm-cloud-rest-api-openapi.yml
  type: http
- description: API key authentication. Provide the API key in the Authorization header obtained from the Sitecore Personalize instance configuration.
  in: header
  name: apiKeyAuth
  parameter: Authorization
  sources:
  - openapi/sitecore-personalize-rest-api-openapi.yml
  type: apiKey
slug: sitecore-authentication
source_filename: sitecore-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/sitecore-cdp-rest-api-openapi.yml, openapi/sitecore-content-hub-rest-api-openapi.yml,\n  openapi/sitecore-discover-api-openapi.yml, openapi/sitecore-ordercloud-api-openapi.yml, openapi/sitecore-personalize-rest-api-openapi.yml,\n  openapi/sitecore-xm-cloud-rest-api-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: basicAuth\n  type: http\n  scheme: basic\n  description: HTTP Basic authentication using a client key as the username and an API token\n    as the password. Credentials are obtained from Sitecore CDP Settings > API access.\n  sources:\n  - openapi/sitecore-cdp-rest-api-openapi.yml\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: OAuth 2.0 bearer token obtained from the Content Hub identity provider. Include\n    the token in the Authorization header as 'Bearer {token}'.\n  sources:\n  - openapi/sitecore-content-hub-rest-api-openapi.yml\n\
  \  - openapi/sitecore-discover-api-openapi.yml\n  - openapi/sitecore-ordercloud-api-openapi.yml\n  - openapi/sitecore-xm-cloud-rest-api-openapi.yml\n- name: apiKeyAuth\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: API key authentication. Provide the API key in the Authorization header obtained\n    from the Sitecore Personalize instance configuration.\n  sources:\n  - openapi/sitecore-personalize-rest-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sitecore/refs/heads/main/authentication/sitecore-authentication.yml
summary_line: apiKey/http · 3 schemes
tags: []
---
