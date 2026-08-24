---
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
method: probed
name: Horizon Robotics Authentication
name_suffix: Authentication
oauth_flows: []
overview: Horizon Robotics declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Horizon Robotics
provider_slug: horizon-robotics
scheme_count: 1
schemes:
- applied: true
  evidence: initialize + tools/list + resources/list + resources/read all returned HTTP 200 with valid JSON-RPC results on unauthenticated requests, 2026-08-22.
  id: none
  surface: https://mcp.oe.horizon.auto/mcp
  type: none
slug: horizon-robotics-authentication
source_filename: horizon-robotics-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-22'\nmethod: probed\nsource: https://mcp.oe.horizon.auto/mcp\ndocs: https://github.com/HorizonRobotics/OE-Skills/blob/main/README.en.md\nsummary: >-\n  Horizon Robotics' one publicly reachable machine surface — the Open Explorer MCP\n  server — requires no authentication at all. Anonymous POSTs from plain curl completed\n  `initialize`, `tools/list`, `resources/list` and `resources/read` with no Authorization\n  header, no session token, no client registration and no OAuth challenge. There is no\n  OAuth 2.0 authorization server, no OpenID Connect discovery document, and no API-key\n  scheme anywhere in the published surface. The credentialed wall at Horizon sits one\n  layer out: a developer-portal account is needed to DOWNLOAD the OpenExplorer package,\n  not to CALL the MCP server.\nschemes:\n- id: none\n  surface: https://mcp.oe.horizon.auto/mcp\n  type: none\n  applied: true\n  evidence: >-\n    initialize + tools/list + resources/list + resources/read\
  \ all returned HTTP 200 with\n    valid JSON-RPC results on unauthenticated requests, 2026-08-22.\noauth:\n  supported: false\n  probes:\n  - url: https://mcp.oe.horizon.auto/.well-known/oauth-protected-resource\n    status: 404\n  - url: https://mcp.oe.horizon.auto/.well-known/oauth-authorization-server\n    status: 404\n  - url: https://www.horizon.auto/.well-known/oauth-authorization-server\n    status: 404\nopenid_connect:\n  supported: false\n  probes:\n  - url: https://www.horizon.auto/.well-known/openid-configuration\n    status: 404\n  - url: https://mcp.oe.horizon.auto/.well-known/openid-configuration\n    status: 404\naccount_gates:\n- surface: https://developer.horizon.auto/\n  gate: developer portal account\n  what_it_unlocks: OpenExplorer (OE) package downloads, chip documentation downloads, forum posting\n  login_url: https://developer.horizon.auto/login\n  probe: {url: 'https://developer.horizon.auto/login', status: 200}\n  note: >-\n    Documentation browsing at developer.horizon.auto/docs\
  \ and doc.oe.horizon.auto is\n    readable without an account; the download endpoints are what require one.\n- surface: OEM / production silicon programs\n  gate: commercial agreement with a Horizon Robotics project manager\n  note: Stated in the product-security policy for OEM partners.\nobservations:\n  transport_security:\n    mcp_endpoint_tls: TLSv1.3\n    mcp_endpoint_hsts: false\n    note: >-\n      mcp.oe.horizon.auto serves TLS 1.3 but sends no Strict-Transport-Security header —\n      recorded in security/horizon-robotics-domain-security.yml.\n  exposure_note: >-\n    An unauthenticated, unrate-limited MCP endpoint that performs vector search over\n    indexed codebases and documentation is a real operational surface. It is not named in\n    the in-scope list of the company's own product-security policy.\nx-evidence:\n  fetched: '2026-08-22'\n  urls:\n  - url: https://mcp.oe.horizon.auto/mcp\n    status: 200\n    note: JSON-RPC initialize, anonymous\n  - url: https://developer.horizon.auto/login\n\
  \    status: 200\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/horizon-robotics/refs/heads/main/authentication/horizon-robotics-authentication.yml
summary_line: 1 scheme
tags:
- Company
- Artificial Intelligence
- Automotive
- Autonomous Driving
- Semiconductors
- Robotics
- Edge AI
- Machine Learning
- Model Context Protocol
- Agent Skills
- Developer Tools
- China
---
