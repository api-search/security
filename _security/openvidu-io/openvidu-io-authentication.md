---
anonymous_access: false
api_key_in: []
api_specs:
- filename: openvidu-io-openapi-generated.yml
  format: yaml
  label: OpenVidu API
  slug: openvidu-io-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/openvidu-io/openapi/_ae-authored/openvidu-io-openapi-generated.yml
auth_types: []
description: OpenVidu supports several authentication methods for client applications.
kind: authentication
layout: security
mechanism_count: 3
method: searched
name: OpenVidu Authentication
name_suffix: Authentication
oauth_flows: []
overview: OpenVidu declares 3 security scheme(s) across its OpenAPI definitions.
provider_name: OpenVidu
provider_slug: openvidu-io
scheme_count: 3
schemes:
- evidence: 'This is a simple authentication method that uses a username and a password. The client application will send the credentials encoded with Base64 in the Authorization header with Basic prefix as stated below:'
  header: Authorization
  how_to_obtain: The client encodes "username:password" with Base64 and includes it in the Authorization header prefixed by "Basic".
  location: header
  name: Basic authentication
  type: http-basic
- evidence: The client stores the token in the browser's local storage and sends it in every request to the server.
  header: Authorization
  how_to_obtain: The application server validates user credentials and returns a signed JWT token, which the client then includes in the Authorization header prefixed by "Bearer".
  location: header
  name: Token-based authentication (JWT)
  type: http-bearer
- evidence: The server application will create a session ID and store it (statefully) in a cookie and return it to the client-side via a cookie header.
  header: Cookie
  how_to_obtain: The server generates a session ID, sends it in a Set-Cookie header, and the client includes the cookie in subsequent requests.
  location: header
  name: Cookie-based authentication
  type: other
slug: openvidu-io-authentication
source_filename: openvidu-io-authentication.yml
source_heading: Authentication Profile
source_url: https://docs.openvidu.io/en/stable/application-server/user-authentication/
source_yaml: "generated: '2026-11-20'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://docs.openvidu.io/en/stable/application-server/user-authentication/\nsources:\n- https://docs.openvidu.io/en/stable/application-server/user-authentication/\n- https://openvidu.io/latest/docs/reference/access-tokens/index.md\n- https://openvidu.io/latest/docs/reference/access-tokens/\n- https://openvidu.io/latest/meet/getting-started/index.md\ndescription: OpenVidu supports several authentication methods for client applications.\nschemes:\n- type: http-basic\n  name: Basic authentication\n  evidence: 'This is a simple authentication method that uses a username and a password. The client application will send the credentials encoded\n    with Base64 in the Authorization header with Basic prefix as stated below:'\n  location: header\n  header: Authorization\n  how_to_obtain: The client encodes \"username:password\" with Base64 and includes it in the Authorization header prefixed\
  \ by \"Basic\".\n- type: http-bearer\n  name: Token-based authentication (JWT)\n  evidence: The client stores the token in the browser's local storage and sends it in every request to the server.\n  location: header\n  header: Authorization\n  how_to_obtain: The application server validates user credentials and returns a signed JWT token, which the client then includes in the Authorization\n    header prefixed by \"Bearer\".\n- type: other\n  name: Cookie-based authentication\n  evidence: The server application will create a session ID and store it (statefully) in a cookie and return it to the client-side via a cookie\n    header.\n  location: header\n  header: Cookie\n  how_to_obtain: The server generates a session ID, sends it in a Set-Cookie header, and the client includes the cookie in subsequent requests.\ndocs: https://docs.openvidu.io/en/stable/application-server/user-authentication/\n"
source_yaml_url: https://artifacts.apis.io/openvidu-io/authentication/openvidu-io-authentication.yml
summary_line: 3 schemes
tags:
- Company
- Video Conferencing
- WebRTC
- Open Source
- Real-Time
- Enterprise
---
