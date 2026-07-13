---
api_key_in: []
api_specs:
- filename: sirion-openapi.yml
  format: yaml
  label: Sirion Contracts API
  slug: sirion-contracts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sirion/refs/heads/main/openapi/sirion-openapi.yml
- filename: sirion-openapi.yml
  format: yaml
  label: Sirion Contract Requests API
  slug: sirion-contract-requests-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sirion/refs/heads/main/openapi/sirion-openapi.yml
- filename: sirion-openapi.yml
  format: yaml
  label: Sirion Metadata & Clauses API
  slug: sirion-metadata-clauses-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sirion/refs/heads/main/openapi/sirion-openapi.yml
- filename: sirion-openapi.yml
  format: yaml
  label: Sirion Obligations API
  slug: sirion-obligations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sirion/refs/heads/main/openapi/sirion-openapi.yml
- filename: sirion-openapi.yml
  format: yaml
  label: Sirion Suppliers & Counterparties API
  slug: sirion-suppliers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sirion/refs/heads/main/openapi/sirion-openapi.yml
- filename: sirion-openapi.yml
  format: yaml
  label: Sirion Integrations & Webhooks API
  slug: sirion-integrations-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sirion/refs/heads/main/openapi/sirion-openapi.yml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: documented
name: Sirion Authentication
name_suffix: Authentication
oauth_flows: []
overview: Sirion secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Sirion
provider_slug: sirion
scheme_count: 1
schemes:
- description: 'CONFIRMED: Sirion B2B APIs use the OAuth 2.0 client credentials grant. A tenant administrator generates an OAuth Client Id and OAuth Client Secret under Admin 2.0 -> Business API & Integrations (OAuth Client Setup, added in release 2.84 with token permission configuration), and shares them with the integration. The client exchanges them for an access token that is presented as a Bearer token on API requests. MODELED: the exact token URL is tenant-specific and not publicly documented; substitute your tenant''s token endpoint.'
  flow: clientCredentials
  name: oauth2ClientCredentials
  scheme: bearer
  sources:
  - https://www.sirion.ai/integrations/
  - https://www.sirion.ai/library/whats-new/sirion-release-284/
  - https://www.sirion.ai/library/whats-new/sirion-release-286/
  type: oauth2
slug: sirion-authentication
source_filename: sirion-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-12'\nmethod: documented\nsource: >-\n  Sirion public product references (integrations page, release notes 2.84 /\n  2.86). The API reference itself is gated behind tenant authentication.\nsummary:\n  types:\n  - oauth2\nschemes:\n- name: oauth2ClientCredentials\n  type: oauth2\n  flow: clientCredentials\n  scheme: bearer\n  description: >-\n    CONFIRMED: Sirion B2B APIs use the OAuth 2.0 client credentials grant. A\n    tenant administrator generates an OAuth Client Id and OAuth Client Secret\n    under Admin 2.0 -> Business API & Integrations (OAuth Client Setup, added in\n    release 2.84 with token permission configuration), and shares them with the\n    integration. The client exchanges them for an access token that is presented\n    as a Bearer token on API requests. MODELED: the exact token URL is\n    tenant-specific and not publicly documented; substitute your tenant's token\n    endpoint.\n  sources:\n  - https://www.sirion.ai/integrations/\n \
  \ - https://www.sirion.ai/library/whats-new/sirion-release-284/\n  - https://www.sirion.ai/library/whats-new/sirion-release-286/\nnotes: >-\n  Access is enterprise / contract-gated. OAuth client credentials are\n  provisioned per tenant; there is no public self-service key issuance.\nmaintainers:\n- FN: Kin Lane\n  email: kin@apievangelist.com\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sirion/refs/heads/main/authentication/sirion-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Contract Management
- Contract Lifecycle Management
- CLM
- Contracts
- AI
- Enterprise
- Legal
- Agreements
- Supplier Management
- Obligations
---
