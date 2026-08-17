---
api_key_in: []
auth_types:
- http
description: ''
kind: authentication
layout: security
method: searched
name: Atom Authentication
name_suffix: Authentication
oauth_flows: []
overview: ATOM secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: ATOM
provider_slug: atom
scheme_count: 1
schemes:
- description: Static account API token issued from the Atom admin panel, sent on every request to the Atom Customers API, the WhatsApp Templates API and webhook-triggered flows. Scope is the whole account; Atom publishes no per-scope or per-permission model.
  format: Bearer <public token>
  in: header
  name: bearerAuth
  parameter_name: Authorization
  scheme: bearer
  sources:
  - https://soporte.atomchat.io/knowledge/api-de-clientes
  - https://soporte.atomchat.io/knowledge/como-enviar-templates-messages-utilizando-la-api-de-atomchat
  token_management:
    expiry: null
    issued_from: Atom admin panel - Configuracion > Mi Empresa > Configuraciones
    refresh: null
    rotation_policy: null
  type: http
slug: atom-authentication
source_filename: atom-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-14'\nmethod: searched\nsource: https://soporte.atomchat.io/knowledge/api-de-clientes\ndocs: https://soporte.atomchat.io/knowledge/api-de-clientes\ndocs_additional:\n- https://soporte.atomchat.io/knowledge/como-enviar-templates-messages-utilizando-la-api-de-atomchat\n- https://soporte.atomchat.io/knowledge/utiliza-la-api-de-plantillas\n- https://soporte.atomchat.io/knowledge/aprende-a-probar-tu-api-en-postman-y-configurarlas-en-las-peticiones-http-de-atom\n- https://soporte.atomchat.io/knowledge/c%C3%B3mo-integrar-atom-con-crm-no-nativos-o-desarrollos-propios\nnotes: >-\n  No OpenAPI is published for the Atom (atomchat.io) API, so this profile is\n  captured from the provider's knowledge base and CONFIRMED by live\n  unauthenticated probes of the documented API host on 2026-08-14. The 2026-07\n  round left the header name unspecified rather than guessing it; that gap is\n  now closed with observed evidence. Atom authenticates with a static account\n  bearer\
  \ token sent in the standard Authorization header:\n  \"Authorization: Bearer <public token>\". The token is generated in the Atom\n  admin panel (Configuracion > Mi Empresa > Configuraciones, security settings)\n  and the same token authenticates webhook-triggered flows. There is no OAuth 2\n  authorization server, no OpenID Connect discovery, no scopes, no token\n  expiry/refresh contract and no published rotation policy - all four\n  /.well-known auth-discovery paths return 404. The API also does NOT return a\n  WWW-Authenticate challenge on 401, which RFC 6750 requires.\nsummary:\n  types:\n  - http\n  api_key_in: []\n  http_schemes:\n  - bearer\n  oauth2_flows: []\n  scopes_published: false\n  mtls: false\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  in: header\n  parameter_name: Authorization\n  format: 'Bearer <public token>'\n  description: >-\n    Static account API token issued from the Atom admin panel, sent on every\n    request to the Atom Customers API,\
  \ the WhatsApp Templates API and\n    webhook-triggered flows. Scope is the whole account; Atom publishes no\n    per-scope or per-permission model.\n  token_management:\n    issued_from: Atom admin panel - Configuracion > Mi Empresa > Configuraciones\n    expiry: null\n    refresh: null\n    rotation_policy: null\n  sources:\n  - https://soporte.atomchat.io/knowledge/api-de-clientes\n  - https://soporte.atomchat.io/knowledge/como-enviar-templates-messages-utilizando-la-api-de-atomchat\nx-evidence:\n- url: https://us-central1-atomchat-io.cloudfunctions.net/templates\n  method: GET\n  http_status: 401\n  content_type: application/json; charset=utf-8\n  body: >-\n    {\"body\":{\"context\":{\"key\":\"Authorization\",\"label\":\"headers.authorization\"},\n    \"message\":\"No authorization token found\",\"path\":[\"headers.authorization\"],\n    \"type\":\"Unauthorized\"},\"code\":401}\n  fetched: '2026-08-14'\n  note: names Authorization / headers.authorization as the required credential\n\
  - url: https://us-central1-atomchat-io.cloudfunctions.net/clients\n  method: GET\n  http_status: 401\n  body: 'No authorization token found.'\n  fetched: '2026-08-14'\n- url: https://us-central1-atomchat-io.cloudfunctions.net/api/Template/SendMessage\n  method: POST\n  http_status: 401\n  body: 'No authorization token found.'\n  fetched: '2026-08-14'\n- url: https://atomchat.io/.well-known/openid-configuration\n  http_status: 404\n  fetched: '2026-08-14'\n- url: https://atomchat.io/.well-known/oauth-authorization-server\n  http_status: 404\n  fetched: '2026-08-14'\n- url: https://us-central1-atomchat-io.cloudfunctions.net/.well-known/oauth-protected-resource\n  http_status: 404\n  fetched: '2026-08-14'\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/atom/refs/heads/main/authentication/atom-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Messaging
- WhatsApp
- Artificial Intelligence
- Conversational Commerce
- Chatbots
- Sales
- Lead Generation
- Customer Engagement
- Latin America
---
