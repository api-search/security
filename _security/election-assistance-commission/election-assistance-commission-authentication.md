---
anonymous_access: false
api_key_in: []
api_specs:
- filename: election-assistance-commission-jsonapi-openapi.yml
  format: yaml
  label: EAC Content JSON:API
  slug: eac
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/election-assistance-commission/refs/heads/main/openapi/election-assistance-commission-jsonapi-openapi.yml
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 0
method: probed
name: Election Assistance Commission Authentication
name_suffix: Authentication
oauth_flows: []
overview: Election Assistance Commission declares 0 security scheme(s) across its OpenAPI definitions.
provider_name: Election Assistance Commission
provider_slug: election-assistance-commission
scheme_count: 0
schemes: []
slug: election-assistance-commission-authentication
source_filename: election-assistance-commission-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-06'\nmethod: probed\nsource: >-\n  live anonymous probes of https://www.eac.gov/jsonapi on 2026-09-06, plus\n  openapi/election-assistance-commission-jsonapi-openapi.yml\nprovider: Election Assistance Commission\nproviderId: election-assistance-commission\ndocs: null\nsummary: >-\n  The EAC's JSON:API surface requires no authentication of any kind. Every read was\n  performed anonymously with no header, key, cookie or token, and returned HTTP 200\n  with application/vnd.api+json. There is no sign-up, no key issuance, no OAuth\n  authorization server and no developer account — because there is no developer\n  programme. This is the simplest possible auth posture and, for a read-only public\n  records API, the correct one.\nschemes: []\nsecurity_requirement: []\nmodel:\n  anonymous_read: true\n  credentialed_read: not-offered\n  write: not-offered\n  note: >-\n    Drupal's JSON:API module on this site is configured read-only. An anonymous\n    POST /jsonapi/node/article\
  \ returned HTTP 405 \"JSON:API is configured to accept only\n    read operations.\" No credential exists that would unlock a write path for a public\n    caller, so authentication is not merely optional — there is nothing to authenticate for.\nauthorization_visible_in_responses:\n  mechanism: Drupal entity access, applied silently per resource type\n  signal: meta.omitted\n  detail: >-\n    63 of the 216 advertised resource types return HTTP 200 with an empty data array and a\n    meta.omitted block reading \"Some resources have been omitted because of insufficient\n    authorisation\". These are configuration and administrative entities (views, field\n    definitions, user roles, webform definitions) plus three content types the EAC keeps\n    non-public (node--person, node--slideshow_slide, node--state_payment_requirements).\n    A caller sees a 200 and an empty collection, not a 401 or 403 — worth knowing, because\n    an agent that branches on status codes will read \"no records\"\
  \ where the truth is\n    \"not permitted\".\nprobes:\n  - url: https://www.eac.gov/jsonapi\n    method: GET\n    credentials: none\n    status: 200\n  - url: https://www.eac.gov/jsonapi/node/voting_system?page[limit]=1\n    method: GET\n    credentials: none\n    status: 200\n  - url: https://www.eac.gov/jsonapi/node/article\n    method: POST\n    credentials: none\n    status: 405\n  - url: https://www.eac.gov/.well-known/openid-configuration\n    method: GET\n    credentials: none\n    status: 404\n  - url: https://www.eac.gov/.well-known/oauth-authorization-server\n    method: GET\n    credentials: none\n    status: 404\n  - url: https://www.eac.gov/.well-known/oauth-protected-resource\n    method: GET\n    credentials: none\n    status: 404\ntransport_security:\n  https_enforced: true\n  tls_version: TLSv1.3\n  see: security/election-assistance-commission-domain-security.yml\nmaintainers:\n  - FN: Kin Lane\n    email: kin@apievangelist.com\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/election-assistance-commission/refs/heads/main/authentication/election-assistance-commission-authentication.yml
summary_line: 0 schemes
tags:
- Federal-Government
- Elections
- Voting
- Open Data
- Voting-Systems
- Certification
- Government-Data
- JSON-API
- Public-Records
---
