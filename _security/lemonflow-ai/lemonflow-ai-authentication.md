---
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
method: searched
name: Lemonflow Ai Authentication
name_suffix: Authentication
oauth_flows: []
overview: Lemonflow declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Lemonflow
provider_slug: lemonflow-ai
scheme_count: 2
schemes:
- credentials:
  - alias_in_iframe: company
    description: Unique company identifier issued by Lemonflow during onboarding.
    in: element-attribute
    name: company
    required: true
  - alias_in_iframe: public_key
    description: Public API key used to authenticate the embed. Documented explicitly as a configuration selector, not a secret - Lemonflow states it is safe to place in a URL. The matching private key remains server-side at Lemonflow and is never exposed to the host page or its users.
    example_prefix: pk_
    in: element-attribute
    name: public-key
    required: true
  id: widget-public-key
  issuance: Credentials are provisioned by Lemonflow per organisation; there is no self-service key console documented.
  rotation: Not documented.
  surface: Lemonflow Chat Widget
  type: apiKey
- description: Complementary embed control rather than a credential. Partners supply the host origins permitted to frame the chat; Lemonflow configures allowed_origins and the chat service then emits a Content-Security-Policy frame-ancestors header. By default any site may iframe the chat, so this is opt-in hardening.
  example: 'allowed_origins: ["https://www.example.com", "https://app.example.com"]'
  id: host-origin-allowlist
  surface: chat.lemonflow.ai/embed
  type: origin-allowlist
slug: lemonflow-ai-authentication
source_filename: lemonflow-ai-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: https://lemonflow-ai.github.io/lemonflow-docs/protected/integration/widget-integration.html\ndocs: https://lemonflow-ai.github.io/lemonflow-docs/protected/integration/widget-integration.html\nnote: >-\n  Derived from published documentation rather than an OpenAPI securitySchemes block -\n  Lemonflow publishes no OpenAPI definition. There is no OAuth authorization server,\n  no OIDC discovery document and no token endpoint on any Lemonflow host, so no\n  scopes/ artifact is emitted.\nschemes:\n- id: widget-public-key\n  type: apiKey\n  surface: Lemonflow Chat Widget\n  credentials:\n  - name: company\n    in: element-attribute\n    alias_in_iframe: company\n    required: true\n    description: Unique company identifier issued by Lemonflow during onboarding.\n  - name: public-key\n    in: element-attribute\n    alias_in_iframe: public_key\n    required: true\n    example_prefix: pk_\n    description: >-\n      Public API key\
  \ used to authenticate the embed. Documented explicitly as a\n      configuration selector, not a secret - Lemonflow states it is safe to place in a\n      URL. The matching private key remains server-side at Lemonflow and is never\n      exposed to the host page or its users.\n  issuance: Credentials are provisioned by Lemonflow per organisation; there is no\n    self-service key console documented.\n  rotation: Not documented.\n- id: host-origin-allowlist\n  type: origin-allowlist\n  surface: chat.lemonflow.ai/embed\n  description: >-\n    Complementary embed control rather than a credential. Partners supply the host\n    origins permitted to frame the chat; Lemonflow configures allowed_origins and the\n    chat service then emits a Content-Security-Policy frame-ancestors header. By\n    default any site may iframe the chat, so this is opt-in hardening.\n  example: 'allowed_origins: [\"https://www.example.com\", \"https://app.example.com\"]'\nend_user_identity:\n  parameter: user-ref\
  \ (user_ref on the iframe)\n  required: false\n  model: >-\n    Conversations are anonymous by default; the widget makes no attempt to identify the\n    visitor. The host application - the only party that knows who the user is - may\n    pass a stable, opaque identifier (hashed email or internal account ID) so that\n    per-user limits on assistant actions apply. Lemonflow configures which actions are\n    capped, the allowance and the period.\npartner_side_authentication:\n  note: >-\n    Applies to the partner CPMS endpoints Lemonflow consumes, not to Lemonflow's own\n    surface.\n  supported:\n  - oauth2\n  - api-key\n  - custom-header\n  bearer_examples_in_docs: 'Authorization: Bearer {token}'\n  stance: Lemonflow states it supports whatever the partner already uses.\ngaps:\n- No /.well-known/openid-configuration or /.well-known/oauth-authorization-server on\n  any probed host (all 404).\n- No documented key rotation or revocation procedure.\n- No documented public REST API requiring\
  \ server-to-server credentials.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/lemonflow-ai/refs/heads/main/authentication/lemonflow-ai-authentication.yml
summary_line: 2 schemes
tags:
- Company
- Artificial Intelligence
- AI Agents
- Customer Support
- Electric Vehicle Charging
- eMobility
- OCPP
- Chat Widget
- Voice
- Europe
---
