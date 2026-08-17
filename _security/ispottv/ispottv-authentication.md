---
api_key_in: []
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Ispottv Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: iSpot.tv secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: iSpot.tv
provider_slug: ispottv
scheme_count: 1
schemes:
- credential_issuance: Client ID and Client Secret are created by an iSpot account manager / Customer Success representative using internal tooling; there is no self-service credential flow.
  flow: clientCredentials
  grant_type_value: client_credentials
  name: OAuth2ClientCredentials
  parameters:
  - client_id
  - client_secret
  - grant_type
  request_content_type: application/x-www-form-urlencoded
  scopes: []
  scopes_note: iSpot publishes no OAuth scope surface. Authorization is account-scoped — access is limited to the brands/industries in the customer's subscription, discoverable at runtime via filter[access]=1 on /v4/brands and /v4/industries rather than through token scopes.
  sources:
  - https://developer.ispot.tv/documentation/python/base-template
  - https://developer.ispot.tv/documentation/glossary
  - https://developer.ispot.tv/sites/default/files/iSpot_API_Integration_Guide_2023-compressed.pdf
  token_lifetime: 24h
  token_lifetime_note: iSpot documents that a token is valid for 24 hours and asks callers not to mint a new token until the current one has expired.
  token_type: Bearer
  token_url: https://api.ispot.tv/v4/oauth2/token
  type: oauth2
slug: ispottv-authentication
source_filename: ispottv-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: searched\nsource: https://developer.ispot.tv/documentation/python/base-template\ndocs: https://developer.ispot.tv/documentation/glossary\nnote: >-\n  iSpot publishes no OpenAPI, so this profile is read from the provider's own\n  public documentation (the Python base-template sample, the API glossary and the\n  publicly served API Integration Guide PDF) and confirmed against live\n  unauthenticated probes of the token and resource endpoints.\nsummary:\n  types:\n  - oauth2\n  api_key_in: []\n  oauth2_flows:\n  - clientCredentials\nschemes:\n- name: OAuth2ClientCredentials\n  type: oauth2\n  flow: clientCredentials\n  token_url: https://api.ispot.tv/v4/oauth2/token\n  request_content_type: application/x-www-form-urlencoded\n  parameters:\n  - client_id\n  - client_secret\n  - grant_type\n  grant_type_value: client_credentials\n  token_type: Bearer\n  token_lifetime: 24h\n  token_lifetime_note: >-\n    iSpot documents that a token is valid for\
  \ 24 hours and asks callers not to\n    mint a new token until the current one has expired.\n  scopes: []\n  scopes_note: >-\n    iSpot publishes no OAuth scope surface. Authorization is account-scoped —\n    access is limited to the brands/industries in the customer's subscription,\n    discoverable at runtime via filter[access]=1 on /v4/brands and /v4/industries\n    rather than through token scopes.\n  credential_issuance: >-\n    Client ID and Client Secret are created by an iSpot account manager /\n    Customer Success representative using internal tooling; there is no\n    self-service credential flow.\n  sources:\n  - https://developer.ispot.tv/documentation/python/base-template\n  - https://developer.ispot.tv/documentation/glossary\n  - https://developer.ispot.tv/sites/default/files/iSpot_API_Integration_Guide_2023-compressed.pdf\nrequest_authorization:\n  header: Authorization\n  format: 'Bearer <access_token>'\n  additional_headers:\n  - name: iSpot-Version\n    required: false\n\
  \    description: >-\n      Date-stamped API version pin. iSpot's own samples send\n      'iSpot-Version: 2017-08-16'; the live API echoes an 'ispot-version'\n      response header (observed value 2024-09-10 on the token endpoint).\nseparate_credentials:\n  note: >-\n    iSpot states explicitly that REST API credentials are NOT interchangeable\n    with developer-site credentials or iSpot Analytics Dashboard credentials —\n    three distinct credential sets.\n  source: https://developer.ispot.tv/sites/default/files/iSpot_API_Integration_Guide_2023-compressed.pdf\npixel_api:\n  note: >-\n    The measurement ingest surface (pi.ispot.tv / pt.ispot.tv) is not\n    OAuth-protected. It authenticates by possession of a client-specific\n    tracking code (Site ID, format TC-####-#) embedded in the request path.\n  source: https://developer.ispot.tv/documentation/unified-measurement\nx-evidence:\n- url: https://api.ispot.tv/v4/oauth2/token\n  method: POST\n  http_status: 400\n  content_type: application/problem+json\n\
  \  observed: >-\n    Live OAuth 2.0 token endpoint; an empty client_credentials request returns\n    RFC 9457 problem+json with type\n    http://developer.ispot.tv/api/v4/errors/invalid-request\n  fetched: '2026-08-13'\n- url: https://api.ispot.tv/v4/brands\n  method: GET\n  http_status: 401\n  content_type: application/problem+json\n  observed: '{\"title\":\"Authentication Required\",\"type\":\"authentication-required\",\"status\":401}'\n  fetched: '2026-08-13'\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ispottv/refs/heads/main/authentication/ispottv-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Company
- TV Advertising
- Advertising Measurement
- Analytics
- Attribution
- Media
- Marketing
- Streaming
---
