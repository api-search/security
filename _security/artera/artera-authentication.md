---
api_key_in:
- unknown
auth_types:
- oauth2
- apiKey
- saml2
description: ''
kind: authentication
layout: security
method: searched
name: Artera Authentication
name_suffix: Authentication
oauth_flows:
- unknown
overview: Artera secures its APIs with oauth2, apiKey, and saml2 across 3 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the unknown flow(s).
provider_name: Artera
provider_slug: artera
scheme_count: 3
schemes:
- api: Artera Messaging API (MAPI)
  authorization_url: null
  description: '"MAPI leverages Auth 2.0" per Artera''s Messaging API documentation. The specific grant type, authorization and token URLs, and scope list are only published inside the developer portal.'
  flows: null
  name: MAPI OAuth 2.0
  scopes: null
  source: https://knowledge.artera.io/en_US/use-cases-and-add-ons/messaging-api-mapi
  token_url: null
  type: oauth2
- api: Artera Messaging API (MAPI)
  description: Onboarding requires the customer to supply API Keys alongside IP addresses. The parameter name and location (header/query) are not published publicly.
  in: unknown
  name: MAPI API key
  parameter_name: null
  source: https://knowledge.artera.io/en_US/use-cases-and-add-ons/messaging-api-mapi
  type: apiKey
- description: SAML 2.0 SSO for staff users of the Artera web application, with MFA. Tracked as its own component on the Artera status page.
  docs: https://knowledge.artera.io/en_US/technical-specifications/saml-single-sign-on-setup-guide
  name: SAML 2.0 single sign-on
  scope: Artera web application (not the API)
  type: saml2
slug: artera-authentication
source_filename: artera-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-15'\nmethod: searched\nsource: https://knowledge.artera.io/en_US/use-cases-and-add-ons/messaging-api-mapi\ndocs: https://knowledge.artera.io/en_US/technical-specifications/saml-single-sign-on-setup-guide\nnote: >-\n  Derived from Artera's public knowledge base only. No OpenAPI is published, so\n  there are no machine-readable securitySchemes to derive from — every scheme\n  below is stated in Artera's own documentation. Token URLs, scopes and grant\n  types are NOT published publicly; they sit behind the registration-gated\n  developer portal, so they are recorded as null rather than guessed.\nsummary:\n  types:\n  - oauth2\n  - apiKey\n  - saml2\n  api_key_in:\n  - unknown\n  oauth2_flows:\n  - unknown\n  network_controls:\n  - ip-allowlist\n  - vpn\nschemes:\n- name: MAPI OAuth 2.0\n  type: oauth2\n  api: Artera Messaging API (MAPI)\n  description: >-\n    \"MAPI leverages Auth 2.0\" per Artera's Messaging API documentation. The\n    specific grant type,\
  \ authorization and token URLs, and scope list are only\n    published inside the developer portal.\n  flows: null\n  authorization_url: null\n  token_url: null\n  scopes: null\n  source: https://knowledge.artera.io/en_US/use-cases-and-add-ons/messaging-api-mapi\n- name: MAPI API key\n  type: apiKey\n  api: Artera Messaging API (MAPI)\n  description: >-\n    Onboarding requires the customer to supply API Keys alongside IP addresses.\n    The parameter name and location (header/query) are not published publicly.\n  in: unknown\n  parameter_name: null\n  source: https://knowledge.artera.io/en_US/use-cases-and-add-ons/messaging-api-mapi\n- name: SAML 2.0 single sign-on\n  type: saml2\n  scope: Artera web application (not the API)\n  description: >-\n    SAML 2.0 SSO for staff users of the Artera web application, with MFA. Tracked\n    as its own component on the Artera status page.\n  docs: https://knowledge.artera.io/en_US/technical-specifications/saml-single-sign-on-setup-guide\nnetwork_controls:\n\
  - control: IP allowlisting\n  applies_to: Artera Messaging API (MAPI)\n  description: Customers supply the IP addresses that will call MAPI during implementation.\n  source: https://knowledge.artera.io/en_US/use-cases-and-add-ons/messaging-api-mapi\n- control: Site-to-site VPN\n  applies_to: EHR/EMR data integration (HL7v2, extracts)\n  description: >-\n    Artera publishes VPN request forms for US and Canadian deployments as part of\n    its technical specification pack.\n  source: https://knowledge.artera.io/en_US/technical-specifications/1239793-technical-specifications\ngaps:\n- >-\n  No /.well-known/openid-configuration or /.well-known/oauth-authorization-server\n  is served on any Artera host (all probed 404) — the OAuth 2.0 metadata an agent\n  would use for automatic discovery does not exist publicly.\n- >-\n  No scope list is published, so scopes/artera-scopes.yml is intentionally absent\n  rather than fabricated.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/artera/refs/heads/main/authentication/artera-authentication.yml
summary_line: oauth2/apiKey/saml2 · 3 schemes
tags:
- Company
- Healthcare
- Patient Communication
- Patient Engagement
- Health IT
- EHR Integration
- FHIR
- Agentic AI
---
