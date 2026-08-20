---
api_key_in:
- header
api_specs:
- filename: lightstream-authenticationservice-api-openapi.yml
  format: yaml
  label: Lightstream AuthenticationService API
  slug: lightstream-authenticationservice-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lightstream/refs/heads/main/openapi/lightstream-authenticationservice-api-openapi.yml
- filename: lightstream-backendauthenticationservice-api-openapi.yml
  format: yaml
  label: Lightstream BackendAuthenticationService API
  slug: lightstream-backendauthenticationservice-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lightstream/refs/heads/main/openapi/lightstream-backendauthenticationservice-api-openapi.yml
- filename: lightstream-collectionservice-api-openapi.yml
  format: yaml
  label: Lightstream CollectionService API
  slug: lightstream-collectionservice-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lightstream/refs/heads/main/openapi/lightstream-collectionservice-api-openapi.yml
- filename: lightstream-destinationservice-api-openapi.yml
  format: yaml
  label: Lightstream DestinationService API
  slug: lightstream-destinationservice-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lightstream/refs/heads/main/openapi/lightstream-destinationservice-api-openapi.yml
- filename: lightstream-eventservice-api-openapi.yml
  format: yaml
  label: Lightstream EventService API
  slug: lightstream-eventservice-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lightstream/refs/heads/main/openapi/lightstream-eventservice-api-openapi.yml
- filename: lightstream-layerservice-api-openapi.yml
  format: yaml
  label: Lightstream LayerService API
  slug: lightstream-layerservice-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lightstream/refs/heads/main/openapi/lightstream-layerservice-api-openapi.yml
- filename: lightstream-layoutservice-api-openapi.yml
  format: yaml
  label: Lightstream LayoutService API
  slug: lightstream-layoutservice-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lightstream/refs/heads/main/openapi/lightstream-layoutservice-api-openapi.yml
- filename: lightstream-projectservice-api-openapi.yml
  format: yaml
  label: Lightstream ProjectService API
  slug: lightstream-projectservice-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lightstream/refs/heads/main/openapi/lightstream-projectservice-api-openapi.yml
- filename: lightstream-publicauthenticationservice-api-openapi.yml
  format: yaml
  label: Lightstream PublicAuthenticationService API
  slug: lightstream-publicauthenticationservice-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lightstream/refs/heads/main/openapi/lightstream-publicauthenticationservice-api-openapi.yml
- filename: lightstream-sourceservice-api-openapi.yml
  format: yaml
  label: Lightstream SourceService API
  slug: lightstream-sourceservice-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lightstream/refs/heads/main/openapi/lightstream-sourceservice-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Lightstream Authentication
name_suffix: Authentication
oauth_flows: []
overview: Lightstream secures its APIs with apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Lightstream
provider_slug: lightstream
scheme_count: 2
schemes:
- description: 'Assert your access token into a HTTP Header named ''Authorization: Bearer''<br><pre>curl -H ''Authorization: Bearer bar'' https://live.api.stream/live/v2/collection/foo</pre>'
  in: header
  name: AccessToken
  parameter: 'Authorization: Bearer'
  sources:
  - openapi/lightstream-live-openapi-original.yml
  type: apiKey
- description: Assert your api key into a HTTP Header named 'X-API-Key'<br><pre>curl -H 'X-API-Key:bar' https://live.api.stream/live/v2/collection/foo</pre>
  in: header
  name: ApiKey
  parameter: X-API-Key
  sources:
  - openapi/lightstream-live-openapi-original.yml
  type: apiKey
slug: lightstream-authentication
source_filename: lightstream-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: derived\nsource: openapi/lightstream-live-openapi-original.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: AccessToken\n  type: apiKey\n  in: header\n  parameter: 'Authorization: Bearer'\n  description: 'Assert your access token into a HTTP Header named ''Authorization: Bearer''<br><pre>curl\n    -H ''Authorization: Bearer bar'' https://live.api.stream/live/v2/collection/foo</pre>'\n  sources:\n  - openapi/lightstream-live-openapi-original.yml\n- name: ApiKey\n  type: apiKey\n  in: header\n  parameter: X-API-Key\n  description: Assert your api key into a HTTP Header named 'X-API-Key'<br><pre>curl -H 'X-API-Key:bar'\n    https://live.api.stream/live/v2/collection/foo</pre>\n  sources:\n  - openapi/lightstream-live-openapi-original.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/lightstream/refs/heads/main/authentication/lightstream-authentication.yml
summary_line: apiKey · 2 schemes
tags:
- Company
- Video
- Live Streaming
- Broadcasting
- WebRTC
- RTMP
- Media
- Compositing
- Real-Time
- Event
- gRPC
- Creator Tools
---
