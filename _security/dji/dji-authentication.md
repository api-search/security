---
api_key_in: []
auth_types:
- app-credentials
description: DJI developer authentication is application-credential based rather than a documented OpenAPI securityScheme (DJI publishes no machine-readable OpenAPI). A developer registers an application in a DJI developer account to obtain an App Key, App Secret, and App License. SDKs (Mobile, Payload, Onboard, Edge, Windows) are activated at runtime with the App Key / App License bound to the application's bundle/package identifier. The Cloud API additionally uses these application credentials to establish device connectivity, with the reference implementation (DJI-Cloud-API-Demo) brokering device tokens over MQTT/HTTP.
kind: authentication
layout: security
method: searched
name: Dji Authentication
name_suffix: Authentication
oauth_flows: []
overview: DJI secures its APIs with app-credentials across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: DJI
provider_slug: dji
scheme_count: 1
schemes:
- applies_to:
  - Mobile SDK
  - Payload SDK
  - Onboard SDK
  - Edge SDK
  - Windows SDK
  - Cloud API
  description: App Key + App Secret + App License issued per registered application via a DJI developer account; required to activate SDKs and access the Cloud API.
  name: DJI App Credentials
  obtained_via: https://account.dji.com/
  type: app-credentials
slug: dji-authentication
source_filename: dji-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: https://developer.dji.com/\ndocs: https://developer.dji.com/cloud-api\ndescription: >-\n  DJI developer authentication is application-credential based rather than a\n  documented OpenAPI securityScheme (DJI publishes no machine-readable OpenAPI).\n  A developer registers an application in a DJI developer account to obtain an\n  App Key, App Secret, and App License. SDKs (Mobile, Payload, Onboard, Edge,\n  Windows) are activated at runtime with the App Key / App License bound to the\n  application's bundle/package identifier. The Cloud API additionally uses these\n  application credentials to establish device connectivity, with the reference\n  implementation (DJI-Cloud-API-Demo) brokering device tokens over MQTT/HTTP.\nsummary:\n  types: [app-credentials]\n  mechanisms:\n    - App Key\n    - App Secret\n    - App License\nschemes:\n  - name: DJI App Credentials\n    type: app-credentials\n    obtained_via: https://account.dji.com/\n\
  \    description: >-\n      App Key + App Secret + App License issued per registered application via a\n      DJI developer account; required to activate SDKs and access the Cloud API.\n    applies_to:\n      - Mobile SDK\n      - Payload SDK\n      - Onboard SDK\n      - Edge SDK\n      - Windows SDK\n      - Cloud API\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/dji/refs/heads/main/authentication/dji-authentication.yml
summary_line: app-credentials · 1 scheme
tags:
- Company
- Drones
- UAV
- Aerial Imaging
- Robotics
- SDK
- Cloud API
- Geospatial
- Hardware
- Enterprise
- Developer Platform
---
