---
api_key_in:
- header
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Trust3 Ai Authentication
name_suffix: Authentication
oauth_flows: []
overview: Trust3 AI secures its APIs with apiKey across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Trust3 AI
provider_slug: trust3-ai
scheme_count: 3
schemes:
- description: Scoped API keys are generated in the Trust3 console (Settings -> API Keys -> Generate scoped key) with a name, optional description, expiry (7/30/90 days, 1 year, or custom), and a scope. The MCP (read) scope grants read-only access to governance context through the hosted MCP server. Keys are shown once at creation.
  docs: https://docs.trust3ai.com/how-to-guides/mcp-configuration.html
  in: header
  name: Trust3 scoped API key (MCP)
  parameter: x-trust3ai-key
  type: apiKey
- description: AI Assets Collectors running in the customer data plane authenticate every request to the Trust3 API server (the public AI Governance API edge) with a Trust3 API key configured as AI_GOVERNANCE_API_KEY. The API server validates the key and routes allowed calls to Trust3 backend services.
  docs: https://docs.trust3ai.com/platform-concepts/control-data-plane.html
  in: header
  name: Trust3 API key (AI Assets Collector)
  parameter: AI_GOVERNANCE_API_KEY (collector configuration)
  type: apiKey
- description: User access to the Trust3 console supports SAML single sign-on with documented setups for Azure AD, Okta, OneLogin, Ping Identity, and other SAML identity providers.
  docs: https://docs.trust3ai.com/get-started/user-management/sso/
  name: Console SSO (SAML)
  protocol: SAML 2.0
  type: sso
slug: trust3-ai-authentication
source_filename: trust3-ai-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://docs.trust3ai.com/how-to-guides/mcp-configuration.html\ndocs: https://docs.trust3ai.com/how-to-guides/mcp-configuration.html\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\n  sso:\n  - SAML 2.0\nschemes:\n- name: Trust3 scoped API key (MCP)\n  type: apiKey\n  in: header\n  parameter: x-trust3ai-key\n  description: >-\n    Scoped API keys are generated in the Trust3 console (Settings -> API Keys\n    -> Generate scoped key) with a name, optional description, expiry (7/30/90\n    days, 1 year, or custom), and a scope. The MCP (read) scope grants\n    read-only access to governance context through the hosted MCP server.\n    Keys are shown once at creation.\n  docs: https://docs.trust3ai.com/how-to-guides/mcp-configuration.html\n- name: Trust3 API key (AI Assets Collector)\n  type: apiKey\n  in: header\n  parameter: AI_GOVERNANCE_API_KEY (collector configuration)\n  description: >-\n    AI Assets Collectors\
  \ running in the customer data plane authenticate every\n    request to the Trust3 API server (the public AI Governance API edge) with a\n    Trust3 API key configured as AI_GOVERNANCE_API_KEY. The API server\n    validates the key and routes allowed calls to Trust3 backend services.\n  docs: https://docs.trust3ai.com/platform-concepts/control-data-plane.html\n- name: Console SSO (SAML)\n  type: sso\n  protocol: SAML 2.0\n  description: >-\n    User access to the Trust3 console supports SAML single sign-on with\n    documented setups for Azure AD, Okta, OneLogin, Ping Identity, and other\n    SAML identity providers.\n  docs: https://docs.trust3ai.com/get-started/user-management/sso/\nnotes: >-\n  No public OAuth 2.0 / OpenID Connect surface is documented for programmatic\n  API access; the docs site's generic REST API reference page is marked as a\n  placeholder by the provider, so only the API-key and SSO mechanisms\n  documented on real pages are recorded here.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/trust3-ai/refs/heads/main/authentication/trust3-ai-authentication.yml
summary_line: apiKey · 3 schemes
tags:
- Company
- Artificial Intelligence
- AI Governance
- AI Agents
- Agent Security
- MCP Security
- Data Governance
- Compliance
- Observability
- Access Control
---
