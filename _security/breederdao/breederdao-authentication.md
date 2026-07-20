---
api_key_in:
- header
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Breederdao Authentication
name_suffix: Authentication
oauth_flows: []
overview: BreederDAO secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: BreederDAO
provider_slug: breederdao
scheme_count: 1
schemes:
- api: ReadyGamer API
  in: header
  name: ReadyGamerApiKey
  parameter_name: X-API-Key
  sources:
  - https://docs.sovrun.org/build-with-sovrun/readygamer/readygamer-api
  type: apiKey
slug: breederdao-authentication
source_filename: breederdao-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: https://docs.sovrun.org/build-with-sovrun/readygamer/readygamer-api\ndocs: https://docs.sovrun.org/build-with-sovrun/readygamer/readygamer-api\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\n  oauth2_flows: []\n  notes: >-\n    The ReadyGamer API authenticates every request with a custom API key sent in\n    the X-API-Key request header. Keys are issued out-of-band by the ReadyGamer\n    team (access requested via a Google Form); there is no self-serve OAuth or\n    OpenID Connect flow documented. Requests are HTTP POST to\n    https://api.ready-gamer.sovrun.org/api/<game>/<command>/chat.\nschemes:\n- name: ReadyGamerApiKey\n  type: apiKey\n  in: header\n  parameter_name: X-API-Key\n  api: ReadyGamer API\n  sources:\n  - https://docs.sovrun.org/build-with-sovrun/readygamer/readygamer-api\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/breederdao/refs/heads/main/authentication/breederdao-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Web3
- Blockchain
- Gaming
- NFT
- Autonomous Worlds
- AI Agents
- Developer Tools
---
