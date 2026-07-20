---
api_key_in: []
api_specs:
- filename: openapi
  format: yaml
  label: Blend API
  slug: blend-api
  spec_type: OpenAPI
  url: https://developers.blend.com/blend/openapi
auth_types:
- oauth2
- http-bearer
- http-basic
description: ''
kind: authentication
layout: security
method: searched
name: Blend Labs Authentication
name_suffix: Authentication
oauth_flows: []
overview: Blend Labs secures its APIs with oauth2, http-bearer, and http-basic across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Blend Labs
provider_slug: blend-labs
scheme_count: 3
schemes:
- flow: clientCredentials
  name: OAuthToken
  source: https://developers.blend.com/blend/reference/create-oauth-token
  token_note: POST to the Create OAuth Token endpoint with a client ID and password to mint a bearer token used to authenticate subsequent requests.
  token_operation: create-oauth-token
  type: oauth2
- name: BearerAuth
  scheme: bearer
  source: https://developers.blend.com/blend/reference/get-application-data
  type: http
- name: BasicAuth
  scheme: basic
  source: https://developers.blend.com/blend/reference/get-application-data
  type: http
slug: blend-labs-authentication
source_filename: blend-labs-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: https://developers.blend.com/blend/reference/create-oauth-token\ndocs: https://developers.blend.com/blend/docs\nsummary:\n  types: [oauth2, http-bearer, http-basic]\n  tenant_header: blend-target-instance\n  notes: >-\n    Every Blend API request requires the multi-tenant blend-target-instance header\n    (form \"[tenant]~[special instance id]\") in addition to one credential scheme\n    (OAuth bearer token, HTTP bearer, or HTTP basic). The blend-target-instance header\n    replaced deprecated tenant headers effective 2020-10-31.\nschemes:\n- name: OAuthToken\n  type: oauth2\n  flow: clientCredentials\n  token_operation: create-oauth-token\n  token_note: >-\n    POST to the Create OAuth Token endpoint with a client ID and password to mint a\n    bearer token used to authenticate subsequent requests.\n  source: https://developers.blend.com/blend/reference/create-oauth-token\n- name: BearerAuth\n  type: http\n  scheme: bearer\n\
  \  source: https://developers.blend.com/blend/reference/get-application-data\n- name: BasicAuth\n  type: http\n  scheme: basic\n  source: https://developers.blend.com/blend/reference/get-application-data\nrequired_headers:\n- name: blend-target-instance\n  in: header\n  required: true\n  description: >-\n    Multi-tenant target instance selector, format \"[tenant]~[special instance id]\".\n    Mandatory on all API routes.\nenvironments:\n- name: production\n  base_url: https://api.blendlabs.com\n- name: beta\n  base_url: https://api.beta.blendlabs.com\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/blend-labs/refs/heads/main/authentication/blend-labs-authentication.yml
summary_line: oauth2/http-bearer/http-basic · 3 schemes
tags:
- Company
- Financial Services
- Mortgage
- Lending
- Banking
- Digital Banking
- Fintech
- Account Opening
- Mortgage Technology
- Consumer Lending
- Deposit Accounts
- Verification
- eClosing
---
