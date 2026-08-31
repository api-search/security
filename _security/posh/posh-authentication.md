---
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
method: probed
name: Posh Authentication
name_suffix: Authentication
oauth_flows: []
overview: Posh declares 0 security scheme(s) across its OpenAPI definitions.
provider_name: Posh
provider_slug: posh
scheme_count: 0
schemes: []
slug: posh-authentication
source_filename: posh-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-26'\nmethod: probed\nsource: 'live probes of https://api.poshdevelopment.com + https://app.poshdevelopment.com + https://security.posh.ai'\nnote: >-\n  No OpenAPI securitySchemes exist to derive from — Posh publishes no contract — so this profile\n  is built only from observed gateway behaviour and Posh's own security claims. The scheme name,\n  header and token format are NOT recorded because they were not observable, and inventing them\n  would be worse than an honest gap.\npublic_documentation: false\nschemes: []\nobserved:\n  - surface: https://api.poshdevelopment.com/api-docs\n    http_status: 403\n    body: 'RBAC: access denied'\n    content_type: text/plain\n    finding: >-\n      The gateway enforces role-based access control at the edge, ahead of the application error\n      handler. This is a positive signal that authorization is centrally enforced, and it is the\n      wall that makes the API reference unreadable to the public.\n  - surface: https://app.poshdevelopment.com/login\n\
  \    http_status: 200\n    finding: >-\n      The Posh Portal is a browser SPA behind a login form. No OIDC discovery document is served\n      (/.well-known/openid-configuration returns the SPA shell, not a document), so the identity\n      provider could not be identified.\n  - surface: https://api.poshdevelopment.com/.well-known/oauth-authorization-server\n    http_status: 404\n    finding: 'No RFC 8414 authorization-server metadata.'\n  - surface: https://api.poshdevelopment.com/.well-known/openid-configuration\n    http_status: 404\n    finding: 'No OIDC discovery.'\nprovider_claims:\n  - claim: multi-factor authentication\n    source: https://security.posh.ai/\n  - claim: role-based access control\n    source: https://security.posh.ai/\n  - claim: voice-based biometric authentication, opt-in consent only\n    source: https://www.posh.ai/security-privacy-policy\n  - claim: 'multi-factor authentication and core system integration in the Voice Assistant'\n    source: https://www.posh.ai/llms.txt\n\
  embedded_surface_auth:\n  component: Posh Answers web embed\n  mechanism: 'Two opaque public identifiers passed as script-tag data attributes: data-org_id and data-user_key.'\n  source: https://poshie-chat-api.poshdevelopment.com/entry-answers.js\n  note: >-\n    Read from the shipped loader, not from documentation. Both values are also accepted as URL\n    query parameters (posh_org_id, posh_user_key), which means they are public, page-embedded\n    identifiers rather than secrets. They scope the embed to a tenant; they are not API\n    credentials and must not be treated as such.\ngaps:\n  - no public authentication documentation\n  - no OIDC or OAuth discovery document on any host\n  - token format, header name and credential lifecycle all unknown to the public\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/posh/refs/heads/main/authentication/posh-authentication.yml
summary_line: 0 schemes
tags:
- Artificial Intelligence
- Conversational AI
- Agentic AI
- Banking
- Credit Unions
- Financial-Services
- Customer Service
- Contact Center
- Voice
- Chatbots
- Knowledge-Management
- RegTech
---
