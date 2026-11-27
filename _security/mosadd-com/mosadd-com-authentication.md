---
anonymous_access: false
api_key_in: []
auth_types: []
description: Authentication for mosADD agents uses a hub key (a bearer token) sent in the Authorization header.
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: mosADD Authentication
name_suffix: Authentication
oauth_flows: []
overview: mosADD declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: mosADD
provider_slug: mosadd-com
scheme_count: 1
schemes:
- evidence: 'Header: `Authorization: Bearer $MOSADD_API_KEY`'
  header: Authorization
  how_to_obtain: Sign in at https://mosadd.com/keys and mint a key (`mosadd_sk_live_…`). The key is provided once and stored in the MOSADD_API_KEY environment variable.
  location: header
  name: Bearer
  type: http-bearer
slug: mosadd-com-authentication
source_filename: mosadd-com-authentication.yml
source_heading: Authentication Profile
source_url: https://mosadd.com/auth.md
source_yaml: "generated: '2026-11-18'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://mosadd.com/auth.md\nsources:\n- https://mosadd.com/auth.md\n- https://mosadd.com/docs/quickstart\n- https://release-assets.githubusercontent.com/github-production-release-asset/1250805629/efe883ca-ed03-4c77-b930-83194ad25389?sp=r&sv=2018-11-09&sr=b&spr=https&se=2026-11-18T23%3A07%3A41Z&rscd=attachment%3B+filename%3DmosADD-Setup-0.2.57.exe&rsct=application%2Foctet-stream&skoid=96c2d410-5711-43a1-aedd-ab1947aa7ab0&sktid=398a6654-997b-47e9-b12b-9515b896b4de&skt=2026-11-18T22%3A07%3A22Z&ske=2026-11-18T23%3A07%3A41Z&sks=b&skv=2018-11-09&sig=GtFbVNgmCyiE8L3LIuokvCgNV8%2BPCmInuSFGvo8g0Dc%3D&jwt=eyJ0eXAiOiJKV1QiLCJhbGciOiJIUzI1NiJ9.eyJpc3MiOiJnaXRodWIuY29tIiwiYXVkIjoicmVsZWFzZS1hc3NldHMuZ2l0aHVidXNlcmNvbnRlbnQuY29tIiwia2V5Ijoia2V5MSIsImV4cCI6MTc5NTA0NDI2NSwibmJmIjoxNzk1MDQwNjY1LCJwYXRoIjoicmVsZWFzZWFzc2V0cHJvZHVjdGlvbi5ibG9iLmNvcmUud2luZG93cy5uZXQifQ.kI4ozk4L_CyDKHpDw_5m7bFaCF2AWtB_HCxF933PVwg&response-content-disposition=attachment%3B%20filename%3DmosADD-Setup-0.2.57.exe&response-content-type=application%2Foctet-stream\n\
  description: Authentication for mosADD agents uses a hub key (a bearer token) sent in the Authorization header.\nschemes:\n- type: http-bearer\n  name: Bearer\n  evidence: 'Header: `Authorization: Bearer $MOSADD_API_KEY`'\n  location: header\n  header: Authorization\n  how_to_obtain: Sign in at https://mosadd.com/keys and mint a key (`mosadd_sk_live_…`). The key is provided once and stored in the MOSADD_API_KEY\n    environment variable.\nnote: No OAuth flows are defined for this provider.\ndocs: https://mosadd.com/auth.md\n"
source_yaml_url: https://artifacts.apis.io/mosadd-com/authentication/mosadd-com-authentication.yml
summary_line: 1 scheme
tags:
- Company
- Artificial Intelligence
- Messaging
- Collaboration
- Security
- AgentOps
---
