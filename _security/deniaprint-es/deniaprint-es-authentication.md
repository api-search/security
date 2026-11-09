---
anonymous_access: true
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Deniaprint Es Authentication
name_suffix: Authentication
oauth_flows: []
overview: Denia Print declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Denia Print
provider_slug: deniaprint-es
scheme_count: 2
schemes:
- applies_to: https://deniaprint.es/mcp
  evidence: 'Servidor MCP (Model Context Protocol), Streamable HTTP, JSON-RPC 2.0, sin autenticación: https://deniaprint.es/mcp.'
  name: anonymous
  type: none
- applies_to:
  - order_status
  - send_status_link
  - message_team
  evidence: Para un pedido necesita tu referencia y el e-mail del pedido, y el enlace de tu pedido solo llega a tu correo, nunca al chat.
  name: order-reference-and-email
  type: possession-factor
slug: deniaprint-es-authentication
source_filename: deniaprint-es-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-05'\nmethod: searched\nsource: https://deniaprint.es/asistentes-ia\ndocs: https://deniaprint.es/asistentes-ia\nsummary: The only published API surface, the remote MCP connector at https://deniaprint.es/mcp, is documented as requiring no authentication (\"sin autenticación\"; \"Sin cuenta, sin clave y sin instalar nada\"). Order tools (order_status, send_status_link, message_team) are gated by knowledge of the order reference (DP-...) plus the order e-mail, not by a credential; the status link is sent to the customer's e-mail, never to the chat.\nschemes:\n- type: none\n  name: anonymous\n  applies_to: https://deniaprint.es/mcp\n  evidence: \"Servidor MCP (Model Context Protocol), Streamable HTTP, JSON-RPC 2.0, sin autenticación: https://deniaprint.es/mcp.\"\n- type: possession-factor\n  name: order-reference-and-email\n  applies_to: [order_status, send_status_link, message_team]\n  evidence: \"Para un pedido necesita tu referencia y el e-mail del pedido,\
  \ y el enlace de tu pedido solo llega a tu correo, nunca al chat.\"\n"
source_yaml_url: https://artifacts.apis.io/deniaprint-es/authentication/deniaprint-es-authentication.yml
summary_line: 2 schemes
tags:
- Company
- Printing
- Print on Demand
- E-Commerce
- Signage
- Graphic Design
- MCP
- Spain
---
