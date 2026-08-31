---
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
method: searched
name: Saama Authentication
name_suffix: Authentication
oauth_flows: []
overview: Saama declares 0 security scheme(s) across its OpenAPI definitions.
provider_name: Saama
provider_slug: saama
scheme_count: 0
schemes: []
slug: saama-authentication
source_filename: saama-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-26'\nmethod: searched\nsource: >-\n  https://www.saama.com/about/company/security-compliance/ and\n  https://www.saama.com/smart-medical-coding/ (site-wide search for an authentication,\n  API key, token or OAuth reference page)\ndocumented: false\ndocumented_flows: 0\npointer_emitted: false\nnote: >-\n  Saama states that authentication exists but publishes no authentication documentation. There is\n  no auth guide, no token endpoint, no key-issuance flow, no scope list and no example request\n  anywhere on the public site: https://www.saama.com/api/, /developers/ and /docs/ all HTTP 301\n  straight to the homepage, and the page sitemap (103 URLs) contains no reference material. What is\n  recorded below is the sum of every authentication statement the company makes in public, and each\n  one is a PROSE CLAIM on a marketing or compliance page rather than a documented flow. No\n  `Authentication` pointer is wired into apis.yml, for the same reason the WellKnown\
  \ pointer was\n  withheld: that pointer asserts the provider documents authentication as its own topic, and Saama\n  does not - crediting it here would score a page that does not exist.\nplatform_authentication:\n  scope: >-\n    Applies to human sign-in to the Saama Platform UI, not to a programmatic API. Stated on the\n    Security & Compliance page.\n  mechanisms:\n  - name: SAML\n    evidence: >-\n      \"Saama's Platform features SAML, OAuth, and LDAP authentication mechanisms and provide\n      seamless single sign-on\"\n  - name: OAuth\n    evidence: same sentence; no version, grant type, authorization server or scope set is named\n  - name: LDAP\n    evidence: same sentence\n  sso: true\n  federated_identity: true\n  mfa:\n    required_for: critical systems\n    evidence: page states multi-factor authentication is required for critical systems\n  authorization:\n    model: role-based access control\n    evidence: >-\n      Data Hub product page describes \"custom queries across\
  \ multiple layers securely using SQL\n      syntax while maintaining robust privacy and role-based controls\"\napi_authentication:\n  documented: false\n  claimed_scheme: token\n  evidence: >-\n    Smart Medical Coding product page, \"EDC & API integration\" capability card: \"Inbound/outbound\n    APIs, EDC connectors, and token-based authentication.\"\n  url: https://www.saama.com/smart-medical-coding/\n  gaps:\n  - no token format, lifetime or refresh behaviour stated\n  - no token or authorization endpoint published\n  - no key issuance, rotation or revocation process published\n  - no scopes or permissions reference\n  - no example request or header name\n  note: >-\n    This single sentence is the only public evidence that a customer-facing API exists at all. It\n    is consistent with the 2025 Clinical AI Agents announcement (\"connected via APIs\") and the Data\n    Hub's 40-plus pre-built connectors, but none of it is reachable or readable without a tenant.\nsecurity_schemes:\
  \ []\nx-evidence:\n- url: https://www.saama.com/about/company/security-compliance/\n  status: 200\n- url: https://www.saama.com/smart-medical-coding/\n  status: 200\n- url: https://www.saama.com/api/\n  status: 301\n  note: redirects to https://www.saama.com/\n- url: https://www.saama.com/developers/\n  status: 301\n  note: redirects to https://www.saama.com/\n- url: https://www.saama.com/docs/\n  status: 301\n  note: redirects to https://www.saama.com/\n- url: https://www.saama.com/.well-known/oauth-authorization-server\n  status: 200\n  note: WordPress HTML homepage shell, not authorization-server metadata - a miss\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/saama/refs/heads/main/authentication/saama-authentication.yml
summary_line: 0 schemes
tags:
- Life Sciences
- Clinical Trials
- Clinical Data Management
- Analytics
- Artificial Intelligence
- Machine-Learning
- Pharmaceuticals
- Healthcare
- Data Platform
- CDISC
---
