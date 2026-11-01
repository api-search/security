---
anonymous_access: false
api_key_in: []
auth_types: []
description: 'Emby supports two authentication mechanisms: User authentication using a custom Authorization header and an access token returned after login, and API‑Key authentication using a static token.'
kind: authentication
layout: security
mechanism_count: 4
method: searched
name: Emby Authentication
name_suffix: Authentication
oauth_flows: []
overview: Emby declares 4 security scheme(s) across its OpenAPI definitions.
provider_name: Emby
provider_slug: emby
scheme_count: 4
schemes:
- evidence: 'Add the following request header on every request: Authorization=Emby UserId="e8837bc1-ad67-520e-8cd2-f629e3155721", Client="Android", Device="Samsung Galaxy SIII", DeviceId="xxx", Version="1.0.0.0"'
  header: Authorization
  how_to_obtain: Obtain the UserId, Client, Device, DeviceId and Version values from the logged‑in user and client application, then include them in the Authorization header as shown.
  location: header
  name: User Authorization Header
  type: other
- evidence: The return result object will have an AccessToken property. This should be included in all subsequent Http requests using the header X-Emby-Token.
  header: X-Emby-Token
  how_to_obtain: Call /Users/AuthenticateByName with the username and password (pw in request body). The response contains an AccessToken which is then sent in the X-Emby-Token header.
  location: header
  name: User Access Token
  token_url: /Users/AuthenticateByName
  type: other
- evidence: Send the API key string in an http request heaser named X-Emby-Token.
  header: X-Emby-Token
  how_to_obtain: Create an API key in the Emby Server Dashboard under Security and use the generated key as the X-Emby-Token header value.
  location: header
  name: API Key Header
  type: apiKey
- evidence: 'An even easier method is to transmit the API key as a query string parameter name api_key . Example: http://localhost:8096/emby/System/Info?api_key=123456789987654321'
  how_to_obtain: Create an API key in the Emby Server Dashboard under Security and use the generated key as the value of the api_key query parameter.
  location: query
  name: API Key Query
  type: apiKey
slug: emby-authentication
source_filename: emby-authentication.yml
source_heading: Authentication Profile
source_url: https://dev.emby.media/doc/restapi/User-Authentication.html
source_yaml: "generated: '2026-10-28'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://dev.emby.media/doc/restapi/User-Authentication.html\nsources:\n- https://dev.emby.media/doc/restapi/User-Authentication.html\n- https://dev.emby.media/doc/restapi/API-Key-Authentication.html\ndescription: 'Emby supports two authentication mechanisms: User authentication using a custom Authorization header and an access token returned\n  after login, and API‑Key authentication using a static token.'\nschemes:\n- type: other\n  name: User Authorization Header\n  evidence: 'Add the following request header on every request: Authorization=Emby UserId=\"e8837bc1-ad67-520e-8cd2-f629e3155721\", Client=\"Android\",\n    Device=\"Samsung Galaxy SIII\", DeviceId=\"xxx\", Version=\"1.0.0.0\"'\n  location: header\n  header: Authorization\n  how_to_obtain: Obtain the UserId, Client, Device, DeviceId and Version values from the logged‑in user and client application, then include them\n\
  \    in the Authorization header as shown.\n- type: other\n  name: User Access Token\n  evidence: The return result object will have an AccessToken property. This should be included in all subsequent Http requests using the header\n    X-Emby-Token.\n  location: header\n  header: X-Emby-Token\n  token_url: /Users/AuthenticateByName\n  how_to_obtain: Call /Users/AuthenticateByName with the username and password (pw in request body). The response contains an AccessToken which\n    is then sent in the X-Emby-Token header.\n- type: apiKey\n  name: API Key Header\n  evidence: Send the API key string in an http request heaser named X-Emby-Token.\n  location: header\n  header: X-Emby-Token\n  how_to_obtain: Create an API key in the Emby Server Dashboard under Security and use the generated key as the X-Emby-Token header value.\n- type: apiKey\n  name: API Key Query\n  evidence: 'An even easier method is to transmit the API key as a query string parameter name api_key . Example: http://localhost:8096/emby/System/Info?api_key=123456789987654321'\n\
  \  location: query\n  how_to_obtain: Create an API key in the Emby Server Dashboard under Security and use the generated key as the value of the api_key query parameter.\ndocs: https://dev.emby.media/doc/restapi/User-Authentication.html\n"
source_yaml_url: https://artifacts.apis.io/emby/authentication/emby-authentication.yml
summary_line: 4 schemes
tags:
- Media Server
- Personal Media
- Streaming
- Video Library
- Music Library
- Live TV
---
