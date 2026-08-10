---
api_key_in: []
api_specs:
- filename: devialet-audio-settings-api-openapi.yml
  format: yaml
  label: Devialet Audio Settings API
  slug: devialet-audio-settings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/devialet/refs/heads/main/openapi/devialet-audio-settings-api-openapi.yml
- filename: devialet-devices-api-openapi.yml
  format: yaml
  label: Devialet Devices API
  slug: devialet-devices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/devialet/refs/heads/main/openapi/devialet-devices-api-openapi.yml
- filename: devialet-groups-api-openapi.yml
  format: yaml
  label: Devialet Groups API
  slug: devialet-groups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/devialet/refs/heads/main/openapi/devialet-groups-api-openapi.yml
- filename: devialet-playback-api-openapi.yml
  format: yaml
  label: Devialet Playback API
  slug: devialet-playback-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/devialet/refs/heads/main/openapi/devialet-playback-api-openapi.yml
- filename: devialet-sound-control-api-openapi.yml
  format: yaml
  label: Devialet Sound Control API
  slug: devialet-sound-control-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/devialet/refs/heads/main/openapi/devialet-sound-control-api-openapi.yml
- filename: devialet-systems-api-openapi.yml
  format: yaml
  label: Devialet Systems API
  slug: devialet-systems-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/devialet/refs/heads/main/openapi/devialet-systems-api-openapi.yml
auth_types:
- none
description: ''
kind: authentication
layout: security
method: searched
name: Devialet Authentication
name_suffix: Authentication
oauth_flows: []
overview: Devialet secures its APIs with none across 0 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Devialet
provider_slug: devialet
scheme_count: 0
schemes: []
slug: devialet-authentication
source_filename: devialet-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-04'\nmethod: searched\nsource: https://help.devialet.com/hc/en-us/articles/4415207423378-Phantom-s-documentation-for-piloting-them-via-IP\ndocs: https://help.devialet.com/hc/en-us/articles/4415207423378-Phantom-s-documentation-for-piloting-them-via-IP\nsource_document: >-\n  Devialet IP Control — REFERENCE API DOCUMENTATION, Revision 1, December 2021\n  (openapi/_original/devialet-ip-control-r1.pdf), section \"Protocol and authentication methods\"\nsummary:\n  types: [none]\n  api_key_in: []\n  oauth2_flows: []\n  transport_security: none\n  posture: unauthenticated-local-network\nschemes: []\nstatement:\n  quote: 'IP Control uses HTTP protocol. No authentication is required.'\n  source: openapi/_original/devialet-ip-control-r1.pdf\n  page: 6\nmodel:\n  authentication: none\n  authorization: none\n  transport: http\n  tls: false\n  port: 80\n  scope_of_trust: >-\n    Any client that can reach the device on the local network can read state and issue every\n\
  \    documented command, including powerOff, restart, and resetToFactorySettings. There is no\n    credential, token, pairing step, or per-client authorization in IP Control v1.\n  network_boundary: >-\n    The API is served by the device itself and is only reachable on the LAN. Devialet does not\n    operate a cloud endpoint for it, so exposure is bounded by the local network segment rather\n    than by an access control in the API.\ndiscovery:\n  mechanism: mDNS / DNS-SD\n  service_type: _http._tcp\n  txt_filter:\n    manufacturer: Devialet\n    ipControlVersion: '1'\n    path: /ipcontrol/v1\n  port: 80\n  note: >-\n    Clients are told to filter service instances on the TXT record key/value pairs\n    manufacturer=Devialet and ipControlVersion=1, and to use the advertised path value rather\n    than hard-coding /ipcontrol/v1.\nintegrator_notes:\n  - >-\n    Because there is no authentication, the practical control is network segmentation. Devialet's\n    Phantom Reactor Custom technical\
  \ guide recommends a fixed-IP configuration on the integrator\n    network and documents that setup and all internal status monitoring happen over this API.\n  - >-\n    Destructive operations (resetDeviceToFactorySettings, resetSystemToFactorySettings) erase\n    network credentials and, on a Wi-Fi-only deployment, make the device unreachable. They are\n    reachable by any unauthenticated LAN client.\nx-evidence:\n  fetched: '2026-08-04'\n  documentation_url: https://help.devialet.com/hc/en-us/articles/4415207423378-Phantom-s-documentation-for-piloting-them-via-IP\n  documentation_http_status: 403\n  documentation_note: >-\n    The live Help Center article is behind a Cloudflare bot challenge for non-browser clients\n    (HTTP 403). The article and its PDF attachment were retrieved from the Internet Archive\n    snapshot of Devialet's own page.\n  attachment_url: https://help.devialet.com/hc/en-us/article_attachments/4415236063506\n  archived_attachment_url: https://web.archive.org/web/20250712105922if_/https://help.devialet.com/hc/en-us/article_attachments/4415236063506\n\
  \  archived_attachment_http_status: 200\n  content_type: application/pdf\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/devialet/refs/heads/main/authentication/devialet-authentication.yml
summary_line: none · 0 schemes
tags:
- Audio
- Consumer Electronics
- Smart Speakers
- Home Automation
- Custom Installation
- Device Control
- Local Network API
- IoT
- Hardware
- Music
- France
---
