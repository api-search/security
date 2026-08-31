---
api_key_in:
- header
api_specs:
- filename: omnisend-brands-api-openapi.yml
  format: yaml
  label: Omnisend Brands API
  slug: omnisend-brands-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/omnisend/refs/heads/main/openapi/omnisend-brands-api-openapi.yml
- filename: omnisend-campaigns-api-openapi.yml
  format: yaml
  label: Omnisend Campaigns API
  slug: omnisend-campaigns-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/omnisend/refs/heads/main/openapi/omnisend-campaigns-api-openapi.yml
- filename: omnisend-contacts-api-openapi.yml
  format: yaml
  label: Omnisend Contacts API
  slug: omnisend-contacts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/omnisend/refs/heads/main/openapi/omnisend-contacts-api-openapi.yml
- filename: omnisend-events-api-openapi.yml
  format: yaml
  label: Omnisend Events API
  slug: omnisend-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/omnisend/refs/heads/main/openapi/omnisend-events-api-openapi.yml
- filename: omnisend-images-api-openapi.yml
  format: yaml
  label: Omnisend Images API
  slug: omnisend-images-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/omnisend/refs/heads/main/openapi/omnisend-images-api-openapi.yml
- filename: omnisend-products-api-openapi.yml
  format: yaml
  label: Omnisend Products API
  slug: omnisend-products-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/omnisend/refs/heads/main/openapi/omnisend-products-api-openapi.yml
- filename: omnisend-segments-api-openapi.yml
  format: yaml
  label: Omnisend Segments API
  slug: omnisend-segments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/omnisend/refs/heads/main/openapi/omnisend-segments-api-openapi.yml
- filename: omnisend-automations-api-openapi.yml
  format: yaml
  label: Omnisend Automations API
  slug: omnisend-automations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/omnisend/refs/heads/main/openapi/omnisend-automations-api-openapi.yml
- filename: omnisend-event-metadata-api-openapi.yml
  format: yaml
  label: Omnisend Event Metadata API
  slug: omnisend-event-metadata-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/omnisend/refs/heads/main/openapi/omnisend-event-metadata-api-openapi.yml
- filename: omnisend-batch-api-openapi.yml
  format: yaml
  label: Omnisend Batch API
  slug: omnisend-batch-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/omnisend/refs/heads/main/openapi/omnisend-batch-api-openapi.yml
- filename: omnisend-email-content-api-openapi.yml
  format: yaml
  label: Omnisend Email Content API
  slug: omnisend-email-content-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/omnisend/refs/heads/main/openapi/omnisend-email-content-api-openapi.yml
- filename: omnisend-email-templates-api-openapi.yml
  format: yaml
  label: Omnisend Email Templates API
  slug: omnisend-email-templates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/omnisend/refs/heads/main/openapi/omnisend-email-templates-api-openapi.yml
- filename: omnisend-email-universal-layouts-api-openapi.yml
  format: yaml
  label: Omnisend Email Universal Layouts API
  slug: omnisend-email-universal-layouts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/omnisend/refs/heads/main/openapi/omnisend-email-universal-layouts-api-openapi.yml
- filename: omnisend-product-categories-api-openapi.yml
  format: yaml
  label: Omnisend Product Categories API
  slug: omnisend-product-categories-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/omnisend/refs/heads/main/openapi/omnisend-product-categories-api-openapi.yml
- filename: omnisend-reports-api-openapi.yml
  format: yaml
  label: Omnisend Reports API
  slug: omnisend-reports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/omnisend/refs/heads/main/openapi/omnisend-reports-api-openapi.yml
- filename: omnisend-statistics-api-openapi.yml
  format: yaml
  label: Omnisend Statistics API
  slug: omnisend-statistics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/omnisend/refs/heads/main/openapi/omnisend-statistics-api-openapi.yml
auth_types:
- apiKey
- oauth2
description: 'Omnisend accepts two credentials on the same Authorization header, distinguished by prefix: "Omnisend-API-Key {key}" and "Bearer {access-token}". Both are accompanied by a REQUIRED Omnisend-Version header. This changed at version 2026-03-15 — the v3/v5 contract carried the key in a bare X-API-KEY header, which no longer applies to the /api base.'
kind: authentication
layout: security
method: searched
name: Omnisend Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: Omnisend secures its APIs with apiKey and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: Omnisend
provider_slug: omnisend
scheme_count: 2
schemes:
- description: 'API key authentication. Use format: Omnisend-API-Key {api-key}'
  in: header
  name: ApiKeyAuth
  parameter: Authorization
  sources:
  - openapi/omnisend-analytics-api-openapi.yml
  - openapi/omnisend-automations-api-openapi.yml
  - openapi/omnisend-batches-api-openapi.yml
  - openapi/omnisend-brands-api-openapi.yml
  - openapi/omnisend-campaigns-api-openapi.yml
  - openapi/omnisend-contacts-api-openapi.yml
  - openapi/omnisend-emailcontent-api-openapi.yml
  - openapi/omnisend-emailtemplates-api-openapi.yml
  - openapi/omnisend-emailuniversallayouts-api-openapi.yml
  - openapi/omnisend-event-metadata-api-openapi.yml
  - openapi/omnisend-events-api-openapi.yml
  - openapi/omnisend-images-api-openapi.yml
  - openapi/omnisend-productcategories-api-openapi.yml
  - openapi/omnisend-products-api-openapi.yml
  - openapi/omnisend-segments-api-openapi.yml
  type: apiKey
- flows:
  - flow: clientCredentials
    scopes: 0
    tokenUrl: https://app.omnisend.com/oauth2/token
  name: Bearer
  sources:
  - openapi/omnisend-analytics-api-openapi.yml
  - openapi/omnisend-automations-api-openapi.yml
  - openapi/omnisend-batches-api-openapi.yml
  - openapi/omnisend-brands-api-openapi.yml
  - openapi/omnisend-campaigns-api-openapi.yml
  - openapi/omnisend-contacts-api-openapi.yml
  - openapi/omnisend-emailcontent-api-openapi.yml
  - openapi/omnisend-emailtemplates-api-openapi.yml
  - openapi/omnisend-emailuniversallayouts-api-openapi.yml
  - openapi/omnisend-event-metadata-api-openapi.yml
  - openapi/omnisend-events-api-openapi.yml
  - openapi/omnisend-images-api-openapi.yml
  - openapi/omnisend-productcategories-api-openapi.yml
  - openapi/omnisend-products-api-openapi.yml
  - openapi/omnisend-segments-api-openapi.yml
  type: oauth2
slug: omnisend-authentication
source_filename: omnisend-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: searched\nsource: https://api-docs.omnisend.com/reference/authentication, https://api-docs.omnisend.com/reference/oauth, https://api-docs.omnisend.com/reference/getting-started,\n  https://mcp.omnisend.com/.well-known/oauth-authorization-server, and openapi/omnisend-*-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - oauth2\n  api_key_in:\n  - header\n  oauth2_flows:\n  - clientCredentials\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: 'API key authentication. Use format: Omnisend-API-Key {api-key}'\n  sources:\n  - openapi/omnisend-analytics-api-openapi.yml\n  - openapi/omnisend-automations-api-openapi.yml\n  - openapi/omnisend-batches-api-openapi.yml\n  - openapi/omnisend-brands-api-openapi.yml\n  - openapi/omnisend-campaigns-api-openapi.yml\n  - openapi/omnisend-contacts-api-openapi.yml\n  - openapi/omnisend-emailcontent-api-openapi.yml\n  - openapi/omnisend-emailtemplates-api-openapi.yml\n\
  \  - openapi/omnisend-emailuniversallayouts-api-openapi.yml\n  - openapi/omnisend-event-metadata-api-openapi.yml\n  - openapi/omnisend-events-api-openapi.yml\n  - openapi/omnisend-images-api-openapi.yml\n  - openapi/omnisend-productcategories-api-openapi.yml\n  - openapi/omnisend-products-api-openapi.yml\n  - openapi/omnisend-segments-api-openapi.yml\n- name: Bearer\n  type: oauth2\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://app.omnisend.com/oauth2/token\n    scopes: 0\n  sources:\n  - openapi/omnisend-analytics-api-openapi.yml\n  - openapi/omnisend-automations-api-openapi.yml\n  - openapi/omnisend-batches-api-openapi.yml\n  - openapi/omnisend-brands-api-openapi.yml\n  - openapi/omnisend-campaigns-api-openapi.yml\n  - openapi/omnisend-contacts-api-openapi.yml\n  - openapi/omnisend-emailcontent-api-openapi.yml\n  - openapi/omnisend-emailtemplates-api-openapi.yml\n  - openapi/omnisend-emailuniversallayouts-api-openapi.yml\n  - openapi/omnisend-event-metadata-api-openapi.yml\n\
  \  - openapi/omnisend-events-api-openapi.yml\n  - openapi/omnisend-images-api-openapi.yml\n  - openapi/omnisend-productcategories-api-openapi.yml\n  - openapi/omnisend-products-api-openapi.yml\n  - openapi/omnisend-segments-api-openapi.yml\ndocs: https://api-docs.omnisend.com/reference/authentication\ndescription: 'Omnisend accepts two credentials on the same Authorization header, distinguished by prefix: \"Omnisend-API-Key\n  {key}\" and \"Bearer {access-token}\". Both are accompanied by a REQUIRED Omnisend-Version header. This changed at\n  version 2026-03-15 — the v3/v5 contract carried the key in a bare X-API-KEY header, which no longer applies to\n  the /api base.'\ndocumented:\n  api_key:\n    header: Authorization\n    format: Omnisend-API-Key {api-key}\n    issued_at: https://app.omnisend.com/integrations/api-keys\n    self_serve: true\n    note: Shown once at creation and not retrievable afterward. Scoped to a brand.\n    example: 'curl --request GET --url ''https://api.omnisend.com/api/segments''\
  \ --header ''Authorization: Omnisend-API-Key\n      YOUR-API-KEY'' --header ''Omnisend-Version: 2026-03-15'''\n  oauth2:\n    header: Authorization\n    format: Bearer {access-token}\n    grant: authorization_code\n    pkce: S256\n    authorization_endpoint: https://app.omnisend.com/oauth2/authorize\n    token_endpoint: https://app.omnisend.com/oauth2/token\n    revocation_endpoint: https://app.omnisend.com/oauth2/revoke\n    registration_endpoint: https://app.omnisend.com/oauth2/register\n    jwks_uri: https://app.omnisend.com/.well-known/jwks.json\n    client_auth_methods:\n    - none\n    - client_secret_post\n    - client_secret_basic\n    refresh: true\n    token_expiry: documented as effectively never (expires_in 9223372036) unless the user revokes\n    onboarding: Manual — https://forms.gle/axz6ychcELUuPrR28, credentials returned in 1-3 business days.\n    required_for:\n    - POST /brands/current (store connection cannot be done with an API key)\n    scopes: scopes/omnisend-scopes.yml\n\
  \  mcp:\n    endpoint: https://mcp.omnisend.com/v2/mcp\n    challenge: 401 Bearer resource_metadata=\"https://mcp.omnisend.com/.well-known/oauth-protected-resource\"\n    alternate_header: X-Api-Key\n    account_roles_required:\n    - Owner\n    - Admin\n    - Manager\n    - Partner\nrequired_headers:\n- name: Omnisend-Version\n  required: true\n  value: '2026-03-15'\n  note: 'Declared as components.parameters.APIVersionHeader with required: true in all 15 harvested contracts. A\n    retired version returns 410.'\ngaps:\n- securitySchemes are declared in every contract but never applied — no document-level `security` block and no per-operation\n  `security`, so the machine-readable contract does not state which credential any operation needs.\n- The Bearer scheme is modelled in the OpenAPI as a clientCredentials flow with only two scopes, while the documented\n  and live flow is authorization_code with 26 scopes. The spec understates the auth model.\n- No OpenID Connect. /.well-known/openid-configuration\
  \ does not serve a discovery document on any Omnisend host.\n- No mutual TLS, no request signing, and no IP allowlisting documented.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/omnisend/refs/heads/main/authentication/omnisend-authentication.yml
summary_line: apiKey/oauth2 · 2 schemes
tags:
- Email Marketing
- Marketing Automation
- E-Commerce
- SMS Marketing
- Customer Engagement
- Segmentation
- Campaigns
- Forms
- Popups
- Web Push
- Automation Workflows
- Analytics
- MCP
- Agent Ready
- Transactional Messaging
---
