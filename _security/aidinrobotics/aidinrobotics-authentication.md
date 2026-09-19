---
anonymous_access: true
api_key_in: []
auth_types: []
description: 'AIDIN ROBOTICS issues no API credential of any kind. There is no developer account, no key, no OAuth client and no token endpoint anywhere on its hosts. Each of its two interfaces has an access model, and neither is authentication in the usual sense: the network surface is anonymous by design, and the device surface is protected by physical access and Linux capabilities.'
kind: authentication
layout: security
mechanism_count: 1
method: probed
name: Aidinrobotics Authentication
name_suffix: Authentication
oauth_flows: []
overview: AIDIN ROBOTICS declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: AIDIN ROBOTICS
provider_slug: aidinrobotics
scheme_count: 2
schemes:
- authored_by: platform (Wix)
  evidence: 'An unauthenticated POST of initialize returned HTTP 200 with serverInfo, and an unauthenticated tools/list returned HTTP 200 with nine tools and full inputSchemas. No WWW-Authenticate challenge, no 401, no bearer token required. The company''s own llms.txt states it plainly: "MCP 엔드포인트에 연결하는 데 인증이 필요하지 않습니다" — no authentication is required to connect to the MCP endpoint — and "사이트에서 접근 가능한 공개 정보만 이용 가능합니다", only publicly accessible site information is available.'
  id: site-mcp-anonymous
  probed: '2026-09-14'
  session_model: The server sets an mcp-session-id response header and an XSRF-TOKEN cookie scoped to www.aidinrobotics.co.kr. Two of the nine tools (CallWixSiteAPI, ExecuteWixAPI) require a visitorToken argument, minted by the server's own GenerateVisitorToken tool, which itself takes no parameters and needs no credential. So the write path is gated by a token an anonymous caller can mint for itself on demand — a session identifier, not an authorization decision.
  surface: AIDIN ROBOTICS Site MCP (https://www.aidinrobotics.co.kr/_api/mcp)
  type: none
  well_known_metadata: None. /.well-known/oauth-protected-resource and /.well-known/oauth-authorization-server both return HTTP 400 (Wix error shell) on this host — consistent with an endpoint that requires no OAuth. See well-known/aidinrobotics-well-known.yml.
- authored_by: provider
  evidence: 'Documented in docs/en/15_error_messages.md and docs/en/05_can_fd_setup.md rather than probed. The SDK''s access control is the operating system''s: opening the CAN socket needs root or CAP_NET_RAW ("permission denied opening CAN socket on ''<name>'' (need root or CAP_NET_RAW)"), and bringing a DOWN interface up needs CAP_NET_ADMIN, which the SDK will not do on the caller''s behalf — it prints the exact `ip link set` command instead.'
  exclusivity: 'The nearest thing to an authorization check on the wire is a conflict detector: the SDK raises "another master is commanding this hand on <name>" and instructs the operator to leave exactly one process running. Possession of the bus is the credential.'
  id: sdk-os-capability
  probed: null
  surface: AIDIN Hand Gen2 SDK
  type: os-capability
slug: aidinrobotics-authentication
source_filename: aidinrobotics-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-14'\nmethod: probed\nsource: https://www.aidinrobotics.co.kr/_api/mcp\nsource_secondary: https://github.com/aidinrobotics/aidin-hand2-sdk/blob/main/docs/en/15_error_messages.md\ndescription: >-\n  AIDIN ROBOTICS issues no API credential of any kind. There is no developer account, no key, no\n  OAuth client and no token endpoint anywhere on its hosts. Each of its two interfaces has an\n  access model, and neither is authentication in the usual sense: the network surface is anonymous\n  by design, and the device surface is protected by physical access and Linux capabilities.\nschemes:\n- id: site-mcp-anonymous\n  surface: AIDIN ROBOTICS Site MCP (https://www.aidinrobotics.co.kr/_api/mcp)\n  type: none\n  probed: '2026-09-14'\n  evidence: >-\n    An unauthenticated POST of initialize returned HTTP 200 with serverInfo, and an\n    unauthenticated tools/list returned HTTP 200 with nine tools and full inputSchemas. No\n    WWW-Authenticate challenge, no 401, no\
  \ bearer token required. The company's own llms.txt states\n    it plainly: \"MCP 엔드포인트에 연결하는 데 인증이 필요하지 않습니다\" — no authentication is required to\n    connect to the MCP endpoint — and \"사이트에서 접근 가능한 공개 정보만 이용 가능합니다\", only publicly\n    accessible site information is available.\n  session_model: >-\n    The server sets an mcp-session-id response header and an XSRF-TOKEN cookie scoped to\n    www.aidinrobotics.co.kr. Two of the nine tools (CallWixSiteAPI, ExecuteWixAPI) require a\n    visitorToken argument, minted by the server's own GenerateVisitorToken tool, which itself takes\n    no parameters and needs no credential. So the write path is gated by a token an anonymous\n    caller can mint for itself on demand — a session identifier, not an authorization decision.\n  well_known_metadata: >-\n    None. /.well-known/oauth-protected-resource and /.well-known/oauth-authorization-server both\n    return HTTP 400 (Wix error shell) on this host — consistent with an endpoint that requires\
  \ no\n    OAuth. See well-known/aidinrobotics-well-known.yml.\n  authored_by: platform (Wix)\n- id: sdk-os-capability\n  surface: AIDIN Hand Gen2 SDK\n  type: os-capability\n  probed: null\n  evidence: >-\n    Documented in docs/en/15_error_messages.md and docs/en/05_can_fd_setup.md rather than probed.\n    The SDK's access control is the operating system's: opening the CAN socket needs root or\n    CAP_NET_RAW (\"permission denied opening CAN socket on '<name>' (need root or CAP_NET_RAW)\"),\n    and bringing a DOWN interface up needs CAP_NET_ADMIN, which the SDK will not do on the caller's\n    behalf — it prints the exact `ip link set` command instead.\n  exclusivity: >-\n    The nearest thing to an authorization check on the wire is a conflict detector: the SDK raises\n    \"another master is commanding this hand on <name>\" and instructs the operator to leave exactly\n    one process running. Possession of the bus is the credential.\n  authored_by: provider\noauth: false\napi_keys:\
  \ false\nmtls: false\nopenid_connect: false\nsignup_url: null\ncredential_note: >-\n  No sign-up, login, developer console or key-issuance page exists on any AIDIN ROBOTICS host. The\n  commercial motion is a sales contact form (https://www.aidinrobotics.co.kr/en/contact) and an\n  online store; software is obtained by cloning a public GitHub repository under Apache-2.0.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/aidinrobotics/refs/heads/main/authentication/aidinrobotics-authentication.yml
summary_line: 2 schemes
tags:
- Robotics
- Sensors
- Hardware
- Industrial Automation
- Manufacturing
- Force and Torque Sensing
- Cobots
- Humanoid Robotics
- ROS
- SDK
- Company
---
