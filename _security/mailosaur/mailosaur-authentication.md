---
api_key_in: []
api_specs:
- filename: mailosaur-analysis-api-openapi.yml
  format: yaml
  label: Mailosaur Analysis API
  slug: mailosaur-analysis-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mailosaur/refs/heads/main/openapi/mailosaur-analysis-api-openapi.yml
- filename: mailosaur-devices-api-openapi.yml
  format: yaml
  label: Mailosaur Devices API
  slug: mailosaur-devices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mailosaur/refs/heads/main/openapi/mailosaur-devices-api-openapi.yml
- filename: mailosaur-files-api-openapi.yml
  format: yaml
  label: Mailosaur Files API
  slug: mailosaur-files-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mailosaur/refs/heads/main/openapi/mailosaur-files-api-openapi.yml
- filename: mailosaur-messages-api-openapi.yml
  format: yaml
  label: Mailosaur Messages API
  slug: mailosaur-messages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mailosaur/refs/heads/main/openapi/mailosaur-messages-api-openapi.yml
- filename: mailosaur-previews-api-openapi.yml
  format: yaml
  label: Mailosaur Previews API
  slug: mailosaur-previews-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mailosaur/refs/heads/main/openapi/mailosaur-previews-api-openapi.yml
- filename: mailosaur-servers-api-openapi.yml
  format: yaml
  label: Mailosaur Servers API
  slug: mailosaur-servers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mailosaur/refs/heads/main/openapi/mailosaur-servers-api-openapi.yml
- filename: mailosaur-usage-api-openapi.yml
  format: yaml
  label: Mailosaur Usage API
  slug: mailosaur-usage-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mailosaur/refs/heads/main/openapi/mailosaur-usage-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: searched
name: Mailosaur Authentication
name_suffix: Authentication
oauth_flows: []
overview: Mailosaur secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Mailosaur
provider_slug: mailosaur
scheme_count: 1
schemes:
- applied: global
  description: HTTP Basic Auth using your Mailosaur API key as the username and an empty password, or your API key as both username and password.
  name: basicAuth
  scheme: basic
  sources:
  - openapi/mailosaur-analysis-api-openapi.yml
  - openapi/mailosaur-devices-api-openapi.yml
  - openapi/mailosaur-files-api-openapi.yml
  - openapi/mailosaur-messages-api-openapi.yml
  - openapi/mailosaur-previews-api-openapi.yml
  - openapi/mailosaur-servers-api-openapi.yml
  - openapi/mailosaur-usage-api-openapi.yml
  type: http
slug: mailosaur-authentication
source_filename: mailosaur-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-14'\nmethod: searched\ndocs: https://mailosaur.com/docs/managing-your-account/api-keys\nsource: >-\n  https://mailosaur.com/docs/api (Authentication section),\n  https://mailosaur.com/docs/managing-your-account/api-keys,\n  https://mailosaur.com/docs/managing-your-account/sso,\n  https://mailosaur.com/docs/managing-your-account/scim, and the securitySchemes\n  of openapi/mailosaur-analysis-api-openapi.yml, openapi/mailosaur-devices-api-openapi.yml,\n  openapi/mailosaur-files-api-openapi.yml, openapi/mailosaur-messages-api-openapi.yml,\n  openapi/mailosaur-previews-api-openapi.yml, openapi/mailosaur-servers-api-openapi.yml,\n  openapi/mailosaur-usage-api-openapi.yml\nsummary:\n  types:\n  - http\n  http_schemes:\n  - basic\n  api_key_in: []\n  oauth2_flows: []\nschemes:\n- name: basicAuth\n  type: http\n  scheme: basic\n  description: HTTP Basic Auth using your Mailosaur API key as the username and an empty password,\n    or your API key as both username\
  \ and password.\n  applied: global\n  sources:\n  - openapi/mailosaur-analysis-api-openapi.yml\n  - openapi/mailosaur-devices-api-openapi.yml\n  - openapi/mailosaur-files-api-openapi.yml\n  - openapi/mailosaur-messages-api-openapi.yml\n  - openapi/mailosaur-previews-api-openapi.yml\n  - openapi/mailosaur-servers-api-openapi.yml\n  - openapi/mailosaur-usage-api-openapi.yml\ncredentials:\n  kind: api-key\n  transport: HTTP Basic — API key as the username, password left empty\n  example: 'curl https://mailosaur.com/api/servers -u api:YOUR_API_KEY'\n  https_required: true\n  key_types:\n    - name: standard\n      scope: account-wide\n      capabilities: >-\n        Full access to all inboxes and all API operations, including creating and\n        deleting inboxes. Required for account-level surfaces — the Usage API,\n        the Devices (TOTP) API and the SCIM API.\n    - name: server-restricted\n      scope: single inbox (server)\n      capabilities: >-\n        Email and SMS functions on\
  \ one inbox only. Cannot create or delete\n        inboxes. A resource outside the key's scope is indistinguishable from one\n        that does not exist — both answer 404 with an empty body.\n  management:\n    console: https://mailosaur.com/app/keys\n    api_manageable: false\n    note: >-\n      Keys can only be created, revealed and deleted in the dashboard, and only\n      by an Account Administrator. There is no key-management API.\n  rotation:\n    expiry: none\n    note: >-\n      Keys never expire and cannot be renamed. Rotation means creating a\n      replacement and deleting the old key; deletion revokes immediately, so cut\n      over before deleting.\n  limits:\n    max_keys: unlimited\nx-evidence:\n  probed: '2026-08-14'\n  url: https://mailosaur.com/api/servers\n  http_status: 401\n  observation: >-\n    An unauthenticated GET returns 401 with `www-authenticate: Bearer` and\n    content-length 0. The advertised challenge scheme contradicts the documented\n    and working\
  \ Basic scheme, and the empty body means the response carries no\n    diagnostic at all. Recorded as observed; not corrected.\naccount_authentication:\n  note: >-\n    Distinct from API authentication. Dashboard sign-in supports Enterprise SSO\n    via SAML2 or OpenID Connect (documented integrations: Okta, Microsoft Entra),\n    with JIT and SCIM 2.0 provisioning. None of this applies to the REST API,\n    which is API-key-over-Basic only — there is no OAuth surface, and therefore\n    no scopes/ artifact for this provider.\n  sso_docs: https://mailosaur.com/docs/managing-your-account/sso\n  scim_docs: https://mailosaur.com/docs/managing-your-account/scim\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mailosaur/refs/heads/main/authentication/mailosaur-authentication.yml
summary_line: http · 1 scheme
tags:
- Email Testing
- SMS Testing
- Developer Tools
- QA Automation
- CI/CD
- SMTP
- TOTP
- Deliverability
---
