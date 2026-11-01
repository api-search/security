---
anonymous_access: false
api_key_in: []
auth_types: []
description: Authentication mechanisms supported by RESTHeart
kind: authentication
layout: security
mechanism_count: 4
method: searched
name: Restheart Authentication
name_suffix: Authentication
oauth_flows: []
overview: SoftInstigate declares 4 security scheme(s) across its OpenAPI definitions.
provider_name: SoftInstigate
provider_slug: restheart
scheme_count: 4
schemes:
- evidence: JwtAuthenticationMechanism reads a Bearer token.
  header: Authorization
  how_to_obtain: 'Obtain a JWT from the /token endpoint (or other login endpoints) and include it in the Authorization: Bearer <jwt> header.'
  location: header
  name: JWT
  type: http-bearer
- evidence: apiKeyAuthMechanism reads the header and extracts the key.
  header: Authorization
  how_to_obtain: 'Create a key via the API (or admin UI) and send it as Authorization: Bearer rhak_<key>.'
  location: header
  name: API Key
  type: http-bearer
- evidence: 'basicAuthMechanism reads the Authorization: Basic header.'
  header: Authorization
  how_to_obtain: 'Send username and password encoded in Base64 in the Authorization: Basic <credentials> header.'
  location: header
  name: Basic
  type: http-basic
- evidence: Cookie Authentication allows the client browser to store an authentication token in a secure cookie.
  how_to_obtain: Authenticate via Basic (or another method) to receive a Set-Cookie response (rh_auth) and then include that cookie on subsequent requests.
  location: cookie
  name: Cookie
  type: other
slug: restheart-authentication
source_filename: restheart-authentication.yml
source_heading: Authentication Profile
source_url: https://restheart.org/docs/security/authentication/overview
source_yaml: "generated: '2026-10-21'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://restheart.org/docs/security/authentication/overview\nsources:\n- https://restheart.org/docs/security/authentication/overview\n- https://restheart.org/docs/security/authentication/jwt\n- https://restheart.org/docs/security/authentication/cookie\n- https://restheart.org/docs/security/authentication/api-key\ndescription: Authentication mechanisms supported by RESTHeart\nschemes:\n- type: http-bearer\n  name: JWT\n  evidence: JwtAuthenticationMechanism reads a Bearer token.\n  location: header\n  header: Authorization\n  how_to_obtain: 'Obtain a JWT from the /token endpoint (or other login endpoints) and include it in the Authorization: Bearer <jwt> header.'\n- type: http-bearer\n  name: API Key\n  evidence: apiKeyAuthMechanism reads the header and extracts the key.\n  location: header\n  header: Authorization\n  how_to_obtain: 'Create a key via the API (or admin UI) and send\
  \ it as Authorization: Bearer rhak_<key>.'\n- type: http-basic\n  name: Basic\n  evidence: 'basicAuthMechanism reads the Authorization: Basic header.'\n  location: header\n  header: Authorization\n  how_to_obtain: 'Send username and password encoded in Base64 in the Authorization: Basic <credentials> header.'\n- type: other\n  name: Cookie\n  evidence: Cookie Authentication allows the client browser to store an authentication token in a secure cookie.\n  location: cookie\n  how_to_obtain: Authenticate via Basic (or another method) to receive a Set-Cookie response (rh_auth) and then include that cookie on subsequent\n    requests.\ndocs: https://restheart.org/docs/security/authentication/overview\n"
source_yaml_url: https://artifacts.apis.io/restheart/authentication/restheart-authentication.yml
summary_line: 4 schemes
tags:
- Database
- Open Source
- NoSQL
- REST
- GraphQL
---
