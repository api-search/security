---
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
method: searched
name: Agibot Authentication
name_suffix: Authentication
oauth_flows: []
overview: AgiBot declares 0 security scheme(s) across its OpenAPI definitions.
provider_name: AgiBot
provider_slug: agibot
scheme_count: 0
schemes: []
slug: agibot-authentication
source_filename: agibot-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-06'\nmethod: searched\nsource: https://store-account.agibot.com/.well-known/openid-configuration\ndocs: https://store.agibot.com/llms.txt\nnotes: AgiBot has two distinct authentication postures. (1) The AimDK robot protocol carries no authentication\n  in the .proto contract itself — RPC request headers hold only a timestamp and an optional blocking flag;\n  access control is a property of the robot and its local network, not of the protocol. (2) The store\n  commerce surface (UCP/MCP) is anonymous for catalog, cart and checkout tools, and uses OAuth 2.0 / OpenID\n  Connect with PKCE for customer-scoped calls.\nx-evidence:\n  fetched: '2026-08-06'\n  url: https://store-account.agibot.com/.well-known/openid-configuration\n  http_status: 200\nsurfaces:\n- api: agibot:aimdk-protocol\n  scheme: none\n  detail: aimdk.protocol.RequestHeader carries a timestamp; BlockableRequestHeader adds a blocked flag.\n    No token, key or credential field is defined anywhere\
  \ in the 136 published .proto files.\n  source: grpc/aimdk/protocol/common/header.proto\n- api: agibot:aimdk-x2\n  scheme: download\n  detail: The AimDK_X2 SDK is obtained by self-service download from the documentation site (floating\n    panel) or via after-sales technical support. The published documentation does not state a credential,\n    licence key or serial-number gate.\n  source: https://x2-aimdk.agibot.com/en/latest/get_sdk/index.html\n- api: agibot:store-commerce\n  scheme: oauth2 + openIdConnect\n  detail: Anonymous for catalog/cart/checkout MCP tools; bearer token in the Authorization header for\n    customer-scoped calls.\n  issuer: https://shopify.com/authentication/62881759275\n  authorization_endpoint: https://store-account.agibot.com/authentication/oauth/authorize\n  token_endpoint: https://store-account.agibot.com/authentication/oauth/token\n  jwks_uri: https://store-account.agibot.com/.well-known/jwks.json\n  end_session_endpoint: https://store-account.agibot.com/authentication/logout\n\
  \  grant_types:\n  - authorization_code\n  - refresh_token\n  - urn:ietf:params:oauth:grant-type:jwt-bearer\n  response_types:\n  - code\n  pkce:\n  - S256\n  token_endpoint_auth_methods:\n  - client_secret_basic\n  id_token_signing_alg:\n  - RS256\n  bearer_methods:\n  - header\n  protected_resource: https://store.agibot.com\n  source: well-known/agibot-openid-configuration.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/agibot/refs/heads/main/authentication/agibot-authentication.yml
summary_line: 0 schemes
tags:
- Company
- Robotics
- Humanoid Robots
- Embodied AI
- Artificial Intelligence
- Manufacturing
- Hardware
- Middleware
- ROS 2
- gRPC
- Protocol Buffers
- Simulation
- Machine Learning
- Open Source
- Model Context Protocol
- Agentic Commerce
- China
---
