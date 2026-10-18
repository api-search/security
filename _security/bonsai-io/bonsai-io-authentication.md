---
anonymous_access: false
api_key_in: []
api_specs:
- filename: bonsai-io-clusters-api-openapi.yml
  format: yaml
  label: Bonsai Clusters API
  slug: bonsai-io-clusters-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bonsai-io/refs/heads/main/openapi/bonsai-io-clusters-api-openapi.yml
- filename: bonsai-io-plans-api-openapi.yml
  format: yaml
  label: Bonsai Plans API
  slug: bonsai-io-plans-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bonsai-io/refs/heads/main/openapi/bonsai-io-plans-api-openapi.yml
- filename: bonsai-io-releases-api-openapi.yml
  format: yaml
  label: Bonsai Releases API
  slug: bonsai-io-releases-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bonsai-io/refs/heads/main/openapi/bonsai-io-releases-api-openapi.yml
- filename: bonsai-io-spaces-api-openapi.yml
  format: yaml
  label: Bonsai Spaces API
  slug: bonsai-io-spaces-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bonsai-io/refs/heads/main/openapi/bonsai-io-spaces-api-openapi.yml
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Bonsai Io Authentication
name_suffix: Authentication
oauth_flows: []
overview: Bonsai declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Bonsai
provider_slug: bonsai-io
scheme_count: 2
schemes:
- description: 'Authorization: Bearer bonsai_<key>_<secret>. This is the simplest option for a new token.'
  name: bearerAuth
  scheme: bearer
  type: http
- description: 'HTTP Basic Auth: the token''s key and secret as the username and password.'
  name: basicAuth
  scheme: basic
  type: http
slug: bonsai-io-authentication
source_filename: bonsai-io-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "name: Bonsai Cloud API Authentication\ngenerated: '2026-10-14'\nmethod: searched\nsource: https://bonsai.io/docs/api/authentication/overview/\ndocs: https://bonsai.io/docs/api/authentication/overview/\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: 'Authorization: Bearer bonsai_<key>_<secret>. This is the simplest option for a new token.'\n- name: basicAuth\n  type: http\n  scheme: basic\n  description: 'HTTP Basic Auth: the token''s key and secret as the username and password.'\ncredential:\n  format: bonsai_<key>_<secret>\n  issued_from: https://bonsai.io/docs/account/api-tokens\nnotes:\n- 'Send one credential per request: a request with more than one, such as both a Basic and a Bearer credential, is refused.'\n- 'Requests that do not have the proper authentication will receive an HTTP 401: Unauthorized response.'\n- 'A token that authenticates but lacks the scope an API call needs gets an HTTP 403: Forbidden response instead.'\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bonsai-io/refs/heads/main/authentication/bonsai-io-authentication.yml
summary_line: 2 schemes
tags:
- Company
- Search
- Elasticsearch
- OpenSearch
- Managed Service
- Vector Search
- Cloud Infrastructure
---
