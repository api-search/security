---
anonymous_access: false
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 3
method: searched
name: Cooper Pet Care Authentication
name_suffix: Authentication
oauth_flows: []
overview: Cooper Pet Care declares 3 security scheme(s) across its OpenAPI definitions.
provider_name: Cooper Pet Care
provider_slug: cooperpetcare-app
scheme_count: 3
schemes:
- applies_to: Cooper REST API (https://api.cooperpetcare.app) - all endpoints, including public catalog and leads
  description: todos los endpoints REST (incluidos los "públicos" de catálogo y leads) requieren además un header x-api-key provisto a clientes autorizados.
  header: x-api-key
  in: header
  name: apiKey
  self_serve: false
  type: apiKey
- applies_to: Cooper REST API order endpoints (POST /orders, GET /customers/orders, GET /orders/{order_id}, PATCH /orders/{order_id})
  bearer_format: idToken
  description: 'los endpoints autenticados usan Authorization: Bearer <idToken>. El token se obtiene desde la app o el sitio web oficiales de Cooper.'
  name: bearerIdToken
  scheme: bearer
  type: http
- applies_to: Cooper MCP server (https://www.cooperpetcare.app/api/mcp) authenticated tools
  description: Tools con autenticación (OAuth 2.1 + PKCE contra Cognito). Public tools (getServiceCatalog, checkCoverage, findCoopersNearby, getBreeds, getShifts, createLead) need no authentication.
  flow: authorizationCode
  identity_provider: Amazon Cognito
  name: mcpOAuth
  pkce: true
  scopes:
  - mcp.read
  - mcp.write
  type: oauth2
slug: cooperpetcare-app-authentication
source_filename: cooperpetcare-app-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: searched\nsource: https://cooperpetcare.app/llms-full.txt\ndocs: https://cooperpetcare.app/llms-full.txt\nnote: No OpenAPI is published; the profile is read from the provider's llms-full.txt (a filtered subset of its unpublished OpenAPI). No authentication endpoint was called.\nschemes:\n- name: apiKey\n  type: apiKey\n  in: header\n  header: x-api-key\n  applies_to: Cooper REST API (https://api.cooperpetcare.app) - all endpoints, including public catalog and leads\n  description: \"todos los endpoints REST (incluidos los \\\"públicos\\\" de catálogo y leads) requieren además un header x-api-key provisto a clientes autorizados.\"\n  self_serve: false\n- name: bearerIdToken\n  type: http\n  scheme: bearer\n  bearer_format: idToken\n  applies_to: Cooper REST API order endpoints (POST /orders, GET /customers/orders, GET /orders/{order_id}, PATCH /orders/{order_id})\n  description: \"los endpoints autenticados usan Authorization: Bearer <idToken>.\
  \ El token se obtiene desde la app o el sitio web oficiales de Cooper.\"\n- name: mcpOAuth\n  type: oauth2\n  flow: authorizationCode\n  pkce: true\n  identity_provider: Amazon Cognito\n  applies_to: Cooper MCP server (https://www.cooperpetcare.app/api/mcp) authenticated tools\n  scopes: [mcp.read, mcp.write]\n  description: \"Tools con autenticación (OAuth 2.1 + PKCE contra Cognito). Public tools (getServiceCatalog, checkCoverage, findCoopersNearby, getBreeds, getShifts, createLead) need no authentication.\"\naccount_flows: Registration, login (email/password, Google, Apple), password recovery and magic links happen only in the official app and website and are not exposed as public endpoints.\n"
source_yaml_url: https://artifacts.apis.io/cooperpetcare-app/authentication/cooperpetcare-app-authentication.yml
summary_line: 3 schemes
tags:
- Company
- Pet Care
- Dog Walking
- Dog Boarding
- Dog Training
- Marketplace
- Mobile App
- Argentina
- Latin America
- MCP
---
