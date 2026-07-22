---
api_key_in:
- config
auth_types:
- apiKey
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Soul Machines Authentication
name_suffix: Authentication
oauth_flows:
- tokenServer
overview: Soul Machines secures its APIs with apiKey and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the tokenServer flow(s).
provider_name: Soul Machines
provider_slug: soul-machines
scheme_count: 2
schemes:
- auth_mode: 0
  description: API key configured in DDNA Studio persona preferences; supplied to the Web SDK to connect to a persona.
  in: config
  name: ApiKey
  type: apiKey
- auth_mode: 1
  description: JWT issued by a developer-operated token server, exchanged for a Digital Person session on the session server. Used with an orchestration server for non-native NLP or custom backend logic.
  name: TokenServer
  scheme: bearer
  token_endpoint: developer-operated (REACT_APP_TOKEN_URL)
  type: oauth2
slug: soul-machines-authentication
source_filename: soul-machines-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://docs.soulmachines.com/web-sdk/ and https://github.com/soulmachines/react-reference-ui-public\ndocs: https://docs.soulmachines.com/web-sdk/\nsummary:\n  types: [apiKey, oauth2]\n  api_key_in: [config]\n  oauth2_flows: [tokenServer]\n  notes: >-\n    A Digital Person session is authenticated in one of two modes, selected per\n    persona (react-reference-ui REACT_APP_PERSONA_AUTH_MODE): 0 = API key, or\n    1 = token server (JWT). API keys are configured in DDNA Studio persona\n    preferences. Token-server auth is used when an orchestration server handles\n    NLP; the client fetches a short-lived JWT from a token endpoint and presents\n    it to the dh.soulmachines.cloud session server.\nschemes:\n- name: ApiKey\n  type: apiKey\n  in: config\n  description: API key configured in DDNA Studio persona preferences; supplied to the Web SDK to connect to a persona.\n  auth_mode: 0\n- name: TokenServer\n  type: oauth2\n  scheme:\
  \ bearer\n  description: JWT issued by a developer-operated token server, exchanged for a Digital Person session on the session server. Used with an orchestration server for non-native NLP or custom backend logic.\n  auth_mode: 1\n  token_endpoint: developer-operated (REACT_APP_TOKEN_URL)\nsession_server: https://dh.soulmachines.cloud\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/soul-machines/refs/heads/main/authentication/soul-machines-authentication.yml
summary_line: apiKey/oauth2 · 2 schemes
tags:
- Company
- Enterprise
- Artificial Intelligence
- Digital Humans
- Avatars
- Conversational AI
- Customer Experience
- SDK
- Web SDK
---
