---
api_key_in:
- header
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Alcatraz Ai Authentication
name_suffix: Authentication
oauth_flows: []
overview: Alcatraz AI secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Alcatraz AI
provider_slug: alcatraz-ai
scheme_count: 1
schemes:
- applies_to: https://platform.alcatraz.ai/api/v2/
  description: API Keys are generated in the Admin Portal under Accounts > Account Settings > API Keys in order to identify and authorize a third-party project or application to access the Alcatraz Admin Portal API. The key value is displayed in plain text exactly once at creation.
  in: header
  name: x-alcatraz-api-key
  parameter_name: x-alcatraz-api-key
  provisioning: self-service inside the authenticated Admin Portal (customer administrators only)
  rotation: keys can be added and removed from the API Keys table; no documented expiry
  sources:
  - https://support.alcatraz.ai/api-keys
  - https://alcatraz-docs.s3.us-west-2.amazonaws.com/Guides/Alcatraz+AI+Admin+Portal+Guide+v2.5.pdf
  type: apiKey
slug: alcatraz-ai-authentication
source_filename: alcatraz-ai-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-06'\nmethod: searched\nsource: https://support.alcatraz.ai/api-keys\ndocs: https://support.alcatraz.ai/api-keys\nnotes: 'No OpenAPI or Swagger document is published by Alcatraz AI, so this profile is\n  read from the vendor''s own public Admin Portal Guide (v2.5) and Help Center rather\n  than derived from a specification. The endpoint reference itself is only reachable\n  from inside the authenticated Admin Portal via its \"API Docs\" button; the guide directs\n  everyone else to their Alcatraz AI account manager.'\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\n  oauth2_flows: []\n  sso: [openIdConnect, saml2]\nschemes:\n- name: x-alcatraz-api-key\n  type: apiKey\n  in: header\n  parameter_name: x-alcatraz-api-key\n  applies_to: https://platform.alcatraz.ai/api/v2/\n  description: 'API Keys are generated in the Admin Portal under Accounts > Account\n    Settings > API Keys in order to identify and authorize a third-party project or\n    application\
  \ to access the Alcatraz Admin Portal API. The key value is displayed\n    in plain text exactly once at creation.'\n  provisioning: self-service inside the authenticated Admin Portal (customer administrators only)\n  rotation: keys can be added and removed from the API Keys table; no documented expiry\n  sources:\n  - https://support.alcatraz.ai/api-keys\n  - https://alcatraz-docs.s3.us-west-2.amazonaws.com/Guides/Alcatraz+AI+Admin+Portal+Guide+v2.5.pdf\nportal_sso:\n  description: 'Administrator sign-in to the Alcatraz Admin Portal (not the API) supports\n    enterprise single sign-on. This is a human authentication surface, not a machine\n    credential.'\n  mechanisms:\n  - id: openIdConnect\n    docs: https://support.alcatraz.ai/sso-configuration-guide\n  - id: saml2\n    note: Azure AD / Entra ID and SAML\n    docs: https://support.alcatraz.ai/single-sign-on-with-azure-and-saml\n  - id: supported-providers\n    docs: https://support.alcatraz.ai/supported-single-sign-on-providers\n\
  gaps:\n- No public OpenAPI/Swagger description of the API.\n- No documented OAuth 2.0 or OpenID Connect flow for API (machine) access — only a static header API key.\n- No published scope or permission model for API keys, so least-privilege cannot be assessed from public material.\n- No public API reference; endpoint list, parameters and error semantics are behind the Admin Portal login.\nx-evidence:\n- url: https://support.alcatraz.ai/api-keys\n  http_status: 200\n  fetched: '2026-08-06'\n  note: 'Help Center article \"API Keys\" — states an API key is required to integrate\n    with the Alcatraz platform via the REST API, and that further REST API information\n    comes from an Alcatraz AI account manager.'\n- url: https://alcatraz-docs.s3.us-west-2.amazonaws.com/Guides/Alcatraz+AI+Admin+Portal+Guide+v2.5.pdf\n  http_status: 200\n  fetched: '2026-08-06'\n  note: 'Section 3.1.7.2 \"API Key Documentation\": Request URL for Alcatraz AI API is\n    https://platform.alcatraz.ai/api/v2/ ;\
  \ authenticate with the header x-alcatraz-api-key.'\n- url: https://support.alcatraz.ai/3rd-party-integrations\n  http_status: 200\n  fetched: '2026-08-06'\n  note: Lists the OIDC and Azure/SAML SSO configuration guides for portal sign-in.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/alcatraz-ai/refs/heads/main/authentication/alcatraz-ai-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Access Control
- Biometrics
- Facial Authentication
- Physical Security
- Identity
- Internet of Things
- Artificial Intelligence
---
