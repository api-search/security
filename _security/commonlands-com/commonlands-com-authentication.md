---
anonymous_access: true
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Commonlands Optics Authentication
name_suffix: Authentication
oauth_flows: []
overview: Commonlands Optics declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Commonlands Optics
provider_slug: commonlands-com
scheme_count: 2
schemes:
- description: The public MCP endpoint https://mcp.commonlands.com/mcp requires no API key and no sign-in.
  name: none
  quote: 'Commonlands is a remote MCP server: one HTTPS endpoint, no API key and no sign-in.'
  type: none
- description: Owner-bound capability token returned by create_cart (and checkout_access_token by create_checkout); required with the cart ID for get_cart, update_cart, cancel_cart and checkout conversion. Not an account credential.
  in: tool-argument
  name: cart_access_token
  quote: 'Carts are also owner-bound: create_cart returns a cart_access_token , and reads, updates, cancellation, and checkout conversion need both the cart ID and that token.'
  type: resource-token
slug: commonlands-com-authentication
source_filename: commonlands-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: searched\nsource: https://commonlands.com/pages/agentic-mcp-for-m12-lenses-and-optics\ndocs: https://commonlands.com/pages/agentic-mcp-for-m12-lenses-and-optics\nname: Commonlands Optics MCP authentication\nschemes:\n- name: none\n  type: none\n  description: The public MCP endpoint https://mcp.commonlands.com/mcp requires no API key and no sign-in.\n  quote: \"Commonlands is a remote MCP server: one HTTPS endpoint, no API key and no sign-in.\"\n- name: cart_access_token\n  type: resource-token\n  in: tool-argument\n  description: Owner-bound capability token returned by create_cart (and checkout_access_token by create_checkout);\n    required with the cart ID for get_cart, update_cart, cancel_cart and checkout conversion. Not an account credential.\n  quote: \"Carts are also owner-bound: create_cart returns a cart_access_token , and reads, updates, cancellation, and checkout conversion need both the cart ID and that token.\"\nnote: The live\
  \ FoV calculations call an authenticated private backend (AWS Lambda) server-side; the docs instruct agents\n  to call only the MCP endpoint and never the backend directly. No customer credentials are accepted by the public surface.\n"
source_yaml_url: https://artifacts.apis.io/commonlands-com/authentication/commonlands-com-authentication.yml
summary_line: 2 schemes
tags:
- Company
- Optics
- Lenses
- Machine Vision
- Embedded Cameras
- Robotics
- E-Commerce
- MCP
---
