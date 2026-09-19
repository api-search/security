---
anonymous_access: true
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 0
method: probed
name: Graphic Packaging Authentication
name_suffix: Authentication
oauth_flows: []
overview: Graphic Packaging declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Graphic Packaging
provider_slug: graphic-packaging
scheme_count: 1
schemes:
- description: 'No authentication. GET https://careers.graphicpkg.com/api/mcp/jobs?tool=search_jobs returned 200 with a full result set anonymously. CORS is wide open (access-control-allow-origin: *), so the surface is callable from a browser or an agent with no onboarding step.'
  evidence:
    http_status: 200
    observed: '2026-09-12'
    url: https://careers.graphicpkg.com/api/mcp/jobs?tool=search_jobs&pageSize=2
  id: none
  in: null
  name: null
  type: none
slug: graphic-packaging-authentication
source_filename: graphic-packaging-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-12'\nmethod: probed\nsource: https://careers.graphicpkg.com/api/mcp/jobs\napi: graphic-packaging-career-site-job-query-api\nsummary: >-\n  The one unauthenticated API surface on a graphicpkg.com host requires no\n  credential at all. Every documented tool answered anonymously on 2026-09-12\n  with HTTP 200 and no WWW-Authenticate challenge, no API key parameter, and no\n  OAuth metadata anywhere on the host. Everything else Graphic Packaging runs\n  (ODS, ACES, GPI Fiber Furnish Tracker, the Esko WebCenter artwork portal) is a\n  human login wall with no documented programmatic auth.\nschemes:\n  - id: none\n    type: none\n    in: null\n    name: null\n    description: >-\n      No authentication. GET https://careers.graphicpkg.com/api/mcp/jobs?tool=search_jobs\n      returned 200 with a full result set anonymously. CORS is wide open\n      (access-control-allow-origin: *), so the surface is callable from a browser\n      or an agent with no onboarding\
  \ step.\n    evidence:\n      url: https://careers.graphicpkg.com/api/mcp/jobs?tool=search_jobs&pageSize=2\n      http_status: 200\n      observed: '2026-09-12'\noauth:\n  present: false\n  authorization_server_metadata: null\n  note: >-\n    /.well-known/oauth-authorization-server and /.well-known/openid-configuration\n    return 404 on www.graphicpkg.com and an HTML shell on careers.graphicpkg.com —\n    no discovery document is served on any host. See\n    well-known/graphic-packaging-well-known.yml.\ngated_surfaces:\n  - name: ODS (order data system)\n    url: https://ods.graphicpkg.com/ods/Account/Login\n    auth: form login, credentials issued by a Graphic Packaging customer service representative\n    programmatic_access_documented: false\n  - name: ACES\n    url: https://aces.graphicpkg.com/login\n    auth: form login\n    programmatic_access_documented: false\n  - name: GPI Fiber Furnish Tracker\n    url: https://gpifiber.graphicpkg.com/\n    auth: form login\n    programmatic_access_documented:\
  \ false\n  - name: Esko WebCenter (gpeyeview) artwork approval\n    url: https://gpeyeview.graphicpkg.com/WebCenter/\n    auth: form login\n    programmatic_access_documented: false\n    note: >-\n      WebCenter is an Esko product with its own vendor API; nothing Graphic\n      Packaging publishes documents or exposes it, so no contract is claimed here.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/graphic-packaging/refs/heads/main/authentication/graphic-packaging-authentication.yml
summary_line: 1 scheme
tags:
- Fortune 500
- Packaging
- Paperboard
- Sustainability
- Manufacturing
- Consumer Packaging
- Food Service
---
