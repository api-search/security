---
api_key_in:
- header
api_specs:
- filename: campfire-accounts-payable-api-openapi.yml
  format: yaml
  label: Campfire Accounts Payable API
  slug: campfire-accounts-payable-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/campfire/refs/heads/main/openapi/campfire-accounts-payable-api-openapi.yml
- filename: campfire-accounts-receivable-api-openapi.yml
  format: yaml
  label: Campfire Accounts Receivable API
  slug: campfire-accounts-receivable-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/campfire/refs/heads/main/openapi/campfire-accounts-receivable-api-openapi.yml
- filename: campfire-bank-reconciliation-api-openapi.yml
  format: yaml
  label: Campfire Bank Reconciliation API
  slug: campfire-bank-reconciliation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/campfire/refs/heads/main/openapi/campfire-bank-reconciliation-api-openapi.yml
- filename: campfire-cash-management-api-openapi.yml
  format: yaml
  label: Campfire Cash Management API
  slug: campfire-cash-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/campfire/refs/heads/main/openapi/campfire-cash-management-api-openapi.yml
- filename: campfire-coa-api-openapi.yml
  format: yaml
  label: Campfire coa API
  slug: campfire-coa-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/campfire/refs/heads/main/openapi/campfire-coa-api-openapi.yml
- filename: campfire-company-objects-api-openapi.yml
  format: yaml
  label: Campfire Company Objects API
  slug: campfire-company-objects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/campfire/refs/heads/main/openapi/campfire-company-objects-api-openapi.yml
- filename: campfire-core-accounting-api-openapi.yml
  format: yaml
  label: Campfire Core Accounting API
  slug: campfire-core-accounting-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/campfire/refs/heads/main/openapi/campfire-core-accounting-api-openapi.yml
- filename: campfire-custom-fields-api-openapi.yml
  format: yaml
  label: Campfire Custom Fields API
  slug: campfire-custom-fields-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/campfire/refs/heads/main/openapi/campfire-custom-fields-api-openapi.yml
- filename: campfire-financial-statements-api-openapi.yml
  format: yaml
  label: Campfire Financial Statements API
  slug: campfire-financial-statements-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/campfire/refs/heads/main/openapi/campfire-financial-statements-api-openapi.yml
- filename: campfire-integrations-api-openapi.yml
  format: yaml
  label: Campfire Integrations API
  slug: campfire-integrations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/campfire/refs/heads/main/openapi/campfire-integrations-api-openapi.yml
- filename: campfire-revenue-recognition-api-openapi.yml
  format: yaml
  label: Campfire Revenue Recognition API
  slug: campfire-revenue-recognition-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/campfire/refs/heads/main/openapi/campfire-revenue-recognition-api-openapi.yml
- filename: campfire-settings-api-openapi.yml
  format: yaml
  label: Campfire Settings API
  slug: campfire-settings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/campfire/refs/heads/main/openapi/campfire-settings-api-openapi.yml
auth_types:
- apiKey
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Campfire Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- clientCredentials
overview: Campfire secures its APIs with apiKey and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode and clientCredentials flow(s).
provider_name: Campfire
provider_slug: campfire
scheme_count: 2
schemes:
- description: 'Primary auth. Django-Knox token in the Authorization header with the required "Token" prefix (e.g. `Authorization: Token YOUR_API_KEY`). Keys are minted per API user under Settings > API Keys (app.meetcampfire.com/v2/settings/api-keys) and shown only once. Each API user carries a role (admin / clerk / view only) that bounds which endpoints the key can call.

    '
  format: Token <API_KEY>
  in: header
  name: knoxApiToken
  parameter: Authorization
  sources:
  - openapi/campfire-openapi-original.json
  type: apiKey
- description: 'Advertised via /.well-known/oauth-authorization-server and /.well-known/openid-configuration on api.meetcampfire.com. issuer https://api.meetcampfire.com; PKCE S256; dynamic client registration supported. Scopes: openid, email, profile (see scopes/campfire-scopes.yml).

    '
  flows:
  - authorizationUrl: https://api.meetcampfire.com/auth/authorize
    flow: authorizationCode
    tokenUrl: https://api.meetcampfire.com/auth/token
  - flow: clientCredentials
    tokenUrl: https://api.meetcampfire.com/auth/token
  name: OAuth2 / OIDC
  sources:
  - https://api.meetcampfire.com/.well-known/openid-configuration
  type: oauth2
slug: campfire-authentication
source_filename: campfire-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: openapi/campfire-openapi-original.json\ndocs: https://docs.campfire.ai/quickstart\nsummary:\n  types:\n  - apiKey\n  - oauth2\n  api_key_in:\n  - header\n  oauth2_flows:\n  - authorizationCode\n  - clientCredentials\n  primary: apiKey\nschemes:\n- name: knoxApiToken\n  type: apiKey\n  in: header\n  parameter: Authorization\n  format: 'Token <API_KEY>'\n  description: >\n    Primary auth. Django-Knox token in the Authorization header with the required\n    \"Token\" prefix (e.g. `Authorization: Token YOUR_API_KEY`). Keys are minted per\n    API user under Settings > API Keys (app.meetcampfire.com/v2/settings/api-keys)\n    and shown only once. Each API user carries a role (admin / clerk / view only)\n    that bounds which endpoints the key can call.\n  sources:\n  - openapi/campfire-openapi-original.json\n- name: OAuth2 / OIDC\n  type: oauth2\n  description: >\n    Advertised via /.well-known/oauth-authorization-server and\n\
  \    /.well-known/openid-configuration on api.meetcampfire.com. issuer\n    https://api.meetcampfire.com; PKCE S256; dynamic client registration\n    supported. Scopes: openid, email, profile (see scopes/campfire-scopes.yml).\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://api.meetcampfire.com/auth/authorize\n    tokenUrl: https://api.meetcampfire.com/auth/token\n  - flow: clientCredentials\n    tokenUrl: https://api.meetcampfire.com/auth/token\n  sources:\n  - https://api.meetcampfire.com/.well-known/openid-configuration\nroles:\n  - {role: admin, access: All APIs}\n  - {role: clerk, access: View all APIs and post draft entries}\n  - {role: view only, access: GET (read-only) APIs}\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/campfire/refs/heads/main/authentication/campfire-authentication.yml
summary_line: apiKey/oauth2 · 2 schemes
tags:
- Company
- Accounting
- ERP
- Finance
- Revenue Recognition
- Accounts Payable
- Accounts Receivable
- AI
---
