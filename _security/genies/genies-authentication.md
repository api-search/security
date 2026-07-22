---
api_key_in:
- project-registration
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Genies Authentication
name_suffix: Authentication
oauth_flows: []
overview: Genies secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Genies
provider_slug: genies
scheme_count: 1
schemes:
- description: Per-project API key issued from the Genies Developer Hub after registering a project; supplied to the Avatar SDK to authenticate the application.
  name: GeniesProjectApiKey
  obtain: https://hub.genies.com/
  sources:
  - https://docs.genies.com/docs/sdk-avatar/getting-started/
  type: apiKey
slug: genies-authentication
source_filename: genies-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: https://docs.genies.com/docs/sdk-avatar/getting-started/\ndocs: https://hub.genies.com/\nnotes: >-\n  Genies has no public REST/OpenAPI surface; auth is captured from the developer\n  docs. Developers create a Genies account, register a project in the Genies\n  Developer Hub (hub.genies.com), and receive API keys / authentication tokens\n  used by the Unity Avatar SDK to authenticate the app and store Genies data.\n  End users can additionally authenticate to load their personal global avatar.\nsummary:\n  types:\n    - apiKey\n  api_key_in:\n    - project-registration\n  oauth2_flows: []\nschemes:\n  - name: GeniesProjectApiKey\n    type: apiKey\n    description: >-\n      Per-project API key issued from the Genies Developer Hub after registering\n      a project; supplied to the Avatar SDK to authenticate the application.\n    obtain: https://hub.genies.com/\n    sources:\n      - https://docs.genies.com/docs/sdk-avatar/getting-started/\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/genies/refs/heads/main/authentication/genies-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Consumer
- Avatars
- Digital Identity
- Artificial Intelligence
- Gaming
- SDK
- Unity
---
