---
anonymous_access: false
api_key_in: []
api_specs:
- filename: california-attorney-general-openjustice-jsonapi-openapi.yml
  format: yaml
  label: OpenJustice Open Data Portal JSON:API
  slug: openjustice-open-data-portal-jsonapi
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/california-attorney-general/refs/heads/main/openapi/california-attorney-general-openjustice-jsonapi-openapi.yml
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 0
method: probed
name: California Attorney General Authentication
name_suffix: Authentication
oauth_flows: []
overview: California Attorney General declares 0 security scheme(s) across its OpenAPI definitions.
provider_name: California Attorney General
provider_slug: california-attorney-general
scheme_count: 0
schemes: []
slug: california-attorney-general-authentication
source_filename: california-attorney-general-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-17'\nmethod: probed\nsource: live anonymous probes of https://data-openjustice.doj.ca.gov/jsonapi on 2026-09-17, plus openapi/california-attorney-general-openjustice-jsonapi-openapi.yml\nprovider: California Attorney General\nproviderId: california-attorney-general\ndocs: null\nsummary: 'The OpenJustice JSON:API requires no authentication for reads. Every collection and individual read was\n  performed anonymously with no header, key, cookie or token and returned HTTP 200 application/vnd.api+json. There\n  is no sign-up, no key issuance, no OAuth authorization server and no developer account, because there is no developer\n  programme. Writes are a different story from most government Drupal JSON:API sites: the module is NOT configured\n  read-only. Anonymous create is granted on the three feedback content types the site footer posts to (node--signup,\n  node--suggestion, node--bug); every other write route answers 401 ''No authentication credentials provided.''\n\
  \  with no documented way for a member of the public to obtain credentials — those routes exist for DOJ content editors.'\nschemes: []\nsecurity_requirement: []\nmodel:\n  anonymous_read: true\n  credentialed_read: not-offered\n  write: anonymous on node--signup / node--suggestion / node--bug only; credentialed (undocumented, staff) elsewhere\n  note: Empty-body anonymous POST returns 400 \"Empty request body.\" on the three feedback routes (authorisation\n    passed, validation failed) and 401 on every other route probed. No populated write was sent.\nauthorization_visible_in_responses:\n  mechanism: Drupal entity access, applied silently per resource type\n  signal: meta.omitted\n  detail: 32 of the 70 advertised resource types return HTTP 200 with an empty data array and a meta.omitted block.\n    These are configuration entities (views, field definitions, roles, webforms, workflows) plus the three feedback\n    types and node--dataset when paged with page[limit]=1 (its lowest-id node\
  \ is unpublished). A caller sees a 200\n    and an empty collection, not a 401 or 403.\nprobes:\n- url: https://data-openjustice.doj.ca.gov/jsonapi\n  method: GET\n  credentials: none\n  status: 200\n- url: https://data-openjustice.doj.ca.gov/jsonapi/node/dataset\n  method: GET\n  credentials: none\n  status: 200\n- url: https://data-openjustice.doj.ca.gov/jsonapi/node/signup\n  method: POST\n  credentials: none\n  body: (empty)\n  status: 400\n- url: https://data-openjustice.doj.ca.gov/jsonapi/node/suggestion\n  method: POST\n  credentials: none\n  body: (empty)\n  status: 400\n- url: https://data-openjustice.doj.ca.gov/jsonapi/node/bug\n  method: POST\n  credentials: none\n  body: (empty)\n  status: 400\n- url: https://data-openjustice.doj.ca.gov/jsonapi/node/dataset\n  method: POST\n  credentials: none\n  body: (empty)\n  status: 401\n- url: https://data-openjustice.doj.ca.gov/jsonapi/node/stats/1a1dff1d-24e8-4050-a617-8f45dba7445f\n  method: PATCH\n  credentials: none\n  status: 401\n\
  - url: https://data-openjustice.doj.ca.gov/jsonapi/node/dataset/1a1dff1d-24e8-4050-a617-8f45dba7445f\n  method: DELETE\n  credentials: none\n  status: 401\n- url: https://oag.ca.gov/.well-known/openid-configuration\n  method: GET\n  status: 404\n- url: https://oag.ca.gov/.well-known/oauth-authorization-server\n  method: GET\n  status: 404\n- url: https://data-openjustice.doj.ca.gov/.well-known/oauth-authorization-server\n  method: GET\n  status: 301\n  note: redirects to the site root\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/california-attorney-general/refs/heads/main/authentication/california-attorney-general-authentication.yml
summary_line: 0 schemes
tags:
- State-Government
- California
- Criminal Justice
- Open Data
- Law Enforcement
- Crime Statistics
- Government Data
- JSON:API
- Public Records
- Attorney General
---
