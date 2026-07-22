---
api_key_in:
- header
api_specs:
- filename: netter-openapi-original.json
  format: json
  label: Netter API (DMI Backend)
  slug: netter-api-dmi-backend
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/netter/refs/heads/main/openapi/netter-openapi-original.json
auth_types:
- apiKey
- oauth2
- saml2
- scim2
description: ''
kind: authentication
layout: security
method: searched
name: Netter Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Netter secures its APIs with apiKey, oauth2, saml2, and scim2 across 3 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Netter
provider_slug: netter
scheme_count: 3
schemes:
- description: Netter public API keys. Created in Settings -> API keys, shown once at creation, tied to the creating user + active company, and inheriting that user's permissions. Sent as a bearer token on every request. Revoking a key is instant; requests with a revoked key return 401 Unauthorized.
  docs: https://netter.ai/docs/api/api-keys.md
  header: Authorization
  key_prefix: ntr_
  location: header
  manage:
    create: create_api_key_api_v1_api_keys__post
    list: list_api_keys_api_v1_api_keys__get
    revoke: revoke_api_key_api_v1_api_keys__key_id__delete
  name: PublicAPIKey
  scheme: bearer
  type: http
  value_format: Bearer ntr_...
- description: Workforce sign-in via any SAML 2.0 identity provider (Microsoft Entra ID, Okta, Google Workspace, etc.). Platform authentication, not API request auth.
  docs: https://netter.ai/docs/security/single-sign-on.md
  name: SAMLSingleSignOn
  type: saml2
- description: SCIM 2.0 user lifecycle provisioning/deprovisioning from the customer IdP.
  docs: https://netter.ai/docs/security/scim-provisioning.md
  name: SCIMProvisioning
  type: scim2
slug: netter-authentication
source_filename: netter-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: https://netter.ai/docs/api/overview.md\ndocs: https://netter.ai/docs/api/api-keys.md\nnote: >-\n  The published OpenAPI (api.netter.ai/openapi.json, \"DMI Backend\") declares no\n  components.securitySchemes, so this profile is captured from the Netter public\n  API documentation rather than derived from the spec.\nsummary:\n  types: [apiKey, oauth2, saml2, scim2]\n  api_key_in: [header]\n  api_key_scheme: bearer\n  oauth2_flows: [authorizationCode]\nschemes:\n  - name: PublicAPIKey\n    type: http\n    scheme: bearer\n    location: header\n    header: Authorization\n    value_format: 'Bearer ntr_...'\n    key_prefix: ntr_\n    description: >-\n      Netter public API keys. Created in Settings -> API keys, shown once at\n      creation, tied to the creating user + active company, and inheriting that\n      user's permissions. Sent as a bearer token on every request. Revoking a key\n      is instant; requests with a revoked\
  \ key return 401 Unauthorized.\n    manage:\n      create: create_api_key_api_v1_api_keys__post\n      list: list_api_keys_api_v1_api_keys__get\n      revoke: revoke_api_key_api_v1_api_keys__key_id__delete\n    docs: https://netter.ai/docs/api/api-keys.md\n  - name: SAMLSingleSignOn\n    type: saml2\n    description: >-\n      Workforce sign-in via any SAML 2.0 identity provider (Microsoft Entra ID,\n      Okta, Google Workspace, etc.). Platform authentication, not API request auth.\n    docs: https://netter.ai/docs/security/single-sign-on.md\n  - name: SCIMProvisioning\n    type: scim2\n    description: >-\n      SCIM 2.0 user lifecycle provisioning/deprovisioning from the customer IdP.\n    docs: https://netter.ai/docs/security/scim-provisioning.md\nintegration_auth_modes:\n  note: >-\n    Auth modes Netter uses to connect *external* systems into pipelines (secrets\n    are brokered and never touch generated step code).\n  modes:\n    - mode: oauth2\n      broker: Nango\n      providers:\
  \ [Databricks, GitHub, Gmail, Notion, Salesforce, Slack]\n    - mode: jwt-keypair\n      providers: [Snowflake]\n    - mode: host-credentials\n      providers: [PostgreSQL]\n    - mode: api-key\n      providers: [Pappers, INSEE SIRENE]\n  docs: https://netter.ai/docs/integrations/authentication.md\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/netter/refs/heads/main/authentication/netter-authentication.yml
summary_line: apiKey/oauth2/saml2/scim2 · 3 schemes
tags:
- Company
- Data
- Data Platform
- Analytics
- Artificial Intelligence
- Ontology
- Data Integration
- Pipelines
- ETL
- Y Combinator
---
