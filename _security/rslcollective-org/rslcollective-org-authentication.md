---
anonymous_access: false
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 3
method: searched
name: Rslcollective Org Authentication
name_suffix: Authentication
oauth_flows: []
overview: RSL Collective declares 3 security scheme(s) across its OpenAPI definitions.
provider_name: RSL Collective
provider_slug: rslcollective-org
scheme_count: 3
schemes:
- applies_to:
  - POST /token
  - POST /introspect
  - POST /key
  credentials_issuance: '"Each client application that interacts with a License Server is assigned a unique client_id and client_secret by the server operator during registration"'
  description: '"Clients MUST authenticate to all OLP endpoints using the HTTP Basic scheme as defined in [ RFC 7617 ]. The Authorization header MUST contain a Base64-encoded string of the form client_id:client_secret."'
  failure: HTTP 401 with an invalid_client JSON error object
  name: olpClientBasic
  scheme: basic
  type: http
- description: '"This endpoint uses the OAuth 2.0 Token Endpoint defined in [ RFC 6749 ] with the client_credentials grant type." Requests carry grant_type, license (URL-encoded RSL <license> XML), optional license_type and resource. The response returns access_token, token_type "License" and expires_in (0 = non-expiring).'
  flows:
    clientCredentials:
      scopes: {}
      tokenUrl: https://api.rslcollective.org/token
  name: olpClientCredentials
  token_url_note: tokenUrl is the documented /token path joined to the server attribute https://api.rslcollective.org.
  type: oauth2
- description: 'Crawler Authorization Protocol: "It introduces a new authentication scheme, License , which uses the standard Authorization and WWW-Authenticate headers to transmit and validate License Tokens over HTTPS connections." Used by crawlers toward publisher resource servers; failures return 401 Unauthorized or 402 Payment Required with a Link header to the governing RSL license.'
  name: capLicense
  scheme: License
  type: http
slug: rslcollective-org-authentication
source_filename: rslcollective-org-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-27'\nmethod: searched\nsource: https://rslstandard.org/rsl\ndocs: https://rslstandard.org/rsl\nrelated_docs:\n- https://rslstandard.org/guide/license-servers\n- https://rslcollective.org/developers\nsummary: >-\n  The RSL Collective license server (https://api.rslcollective.org, named as the server in the\n  collective's own RSL license examples and listed as an RSL License Server in the RSL Standard guide)\n  is governed by the RSL 1.0 Open License Protocol (OLP), which the collective's editors publish at\n  rslstandard.org. OLP is an OAuth 2.0 extension: clients authenticate to every OLP endpoint with HTTP\n  Basic client credentials and receive an opaque License Token, which they then present to resource\n  servers using the CAP `License` HTTP authentication scheme. Credentials are obtained by joining via the\n  RSL Collective dashboard (\"Join for free to request access to the RSL Collective licensing APIs and\n  tools\"). Not verified against the live\
  \ server: no endpoint was called (auth endpoints are out of scope\n  for probing).\nschemes:\n- name: olpClientBasic\n  type: http\n  scheme: basic\n  applies_to: [POST /token, POST /introspect, POST /key]\n  description: >-\n    \"Clients MUST authenticate to all OLP endpoints using the HTTP Basic scheme as defined in [ RFC 7617 ].\n    The Authorization header MUST contain a Base64-encoded string of the form client_id:client_secret.\"\n  credentials_issuance: >-\n    \"Each client application that interacts with a License Server is assigned a unique client_id and\n    client_secret by the server operator during registration\"\n  failure: HTTP 401 with an invalid_client JSON error object\n- name: olpClientCredentials\n  type: oauth2\n  flows:\n    clientCredentials:\n      tokenUrl: https://api.rslcollective.org/token\n      scopes: {}\n  description: >-\n    \"This endpoint uses the OAuth 2.0 Token Endpoint defined in [ RFC 6749 ] with the client_credentials\n    grant type.\" Requests\
  \ carry grant_type, license (URL-encoded RSL <license> XML), optional license_type\n    and resource. The response returns access_token, token_type \"License\" and expires_in (0 = non-expiring).\n  token_url_note: tokenUrl is the documented /token path joined to the server attribute https://api.rslcollective.org.\n- name: capLicense\n  type: http\n  scheme: License\n  description: >-\n    Crawler Authorization Protocol: \"It introduces a new authentication scheme, License , which uses the\n    standard Authorization and WWW-Authenticate headers to transmit and validate License Tokens over HTTPS\n    connections.\" Used by crawlers toward publisher resource servers; failures return 401 Unauthorized or\n    402 Payment Required with a Link header to the governing RSL license.\n"
source_yaml_url: https://artifacts.apis.io/rslcollective-org/authentication/rslcollective-org-authentication.yml
summary_line: 3 schemes
tags:
- Company
- AI Licensing
- Content Licensing
- Collective Rights
- Publishers
- Royalties
- Nonprofit
- RSL Standard
---
