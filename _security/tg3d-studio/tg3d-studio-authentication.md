---
api_key_in:
- header
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Tg3D Studio Authentication
name_suffix: Authentication
oauth_flows: []
overview: TG3D Studio secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: TG3D Studio
provider_slug: tg3d-studio
scheme_count: 1
schemes:
- description: Partner API key generated in the Scanatic for Fashion Developer Console and sent on each request over HTTPS. Requires an account with Developer permission. Header name not published outside the gated console.
  in: header
  name: apiKey
  sources:
  - https://tg3ds.zendesk.com/hc/en-us/articles/900003496766-Using-the-APIs-in-a-nutshell
  type: apiKey
slug: tg3d-studio-authentication
source_filename: tg3d-studio-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://tg3ds.zendesk.com/hc/en-us/articles/900003496766-Using-the-APIs-in-a-nutshell\ndocs: https://tg3ds.zendesk.com/hc/en-us/categories/900001218663-Business-Integration-with-APIs\nsummary:\n  types: [apiKey]\n  api_key_in: [header]\n  oauth2_flows: []\n  notes: >-\n    TG3D Studio exposes two libraries of RESTful APIs — ScanAPI (free to partners;\n    controls the Scanatic 360 Body Scanner and registers Cloudzet scan users) and\n    APIConnect (manipulates data across the Scanatic Body, Nuno3D and StyleBook\n    services). API access is credential/key based and issued from the Developer\n    Console inside the Scanatic for Fashion (S4F) platform; the account must be\n    granted Developer permission by an Admin before a key can be generated. All\n    HTTPS data flows are 256-bit encrypted. The exact header name and any token\n    exchange are documented only inside the gated Developer Console and were not\n    publicly\
  \ verifiable, so no scheme parameter values are asserted here.\nschemes:\n  - name: apiKey\n    type: apiKey\n    in: header\n    description: >-\n      Partner API key generated in the Scanatic for Fashion Developer Console and\n      sent on each request over HTTPS. Requires an account with Developer\n      permission. Header name not published outside the gated console.\n    sources: [https://tg3ds.zendesk.com/hc/en-us/articles/900003496766-Using-the-APIs-in-a-nutshell]\napis:\n  - name: ScanAPI\n    description: >-\n      Free RESTful API for partners to integrate Cloudzet scan-user registration\n      with their own membership creation and to build their own UI (app or web)\n      that controls the Scanatic 360 Body Scanner.\n  - name: APIConnect\n    description: >-\n      RESTful API offering a wide variety of commands to manipulate data across\n      the Scanatic Body Service, Scanatic Nuno3D Service and Scanatic StyleBook\n      Service.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tg3d-studio/refs/heads/main/authentication/tg3d-studio-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- 3D Body Scanning
- Fashion Technology
- Made-to-Measure
- Digital Fashion
- Body Measurement
- Apparel
- API
---
