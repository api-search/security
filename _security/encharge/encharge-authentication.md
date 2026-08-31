---
api_key_in:
- header
- query
api_specs:
- filename: TVRj5o3E
  format: yaml
  label: Encharge Transactional Email API
  slug: transactional-email-api
  spec_type: Postman
  url: https://documenter.getpostman.com/view/460427/TVRj5o3E
- filename: SVfNwVFU
  format: yaml
  label: Encharge Ingest API
  slug: ingest-api
  spec_type: Postman
  url: https://documenter.getpostman.com/view/460427/SVfNwVFU
- filename: encharge-account-api-openapi.yml
  format: yaml
  label: Encharge Account API
  slug: encharge-account-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/encharge/refs/heads/main/openapi/encharge-account-api-openapi.yml
- filename: encharge-broadcasts-api-openapi.yml
  format: yaml
  label: Encharge Broadcasts API
  slug: encharge-broadcasts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/encharge/refs/heads/main/openapi/encharge-broadcasts-api-openapi.yml
- filename: encharge-customobjects-api-openapi.yml
  format: yaml
  label: Encharge Custom Objects API
  slug: encharge-customobjects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/encharge/refs/heads/main/openapi/encharge-customobjects-api-openapi.yml
- filename: encharge-customobjectsschema-api-openapi.yml
  format: yaml
  label: Encharge Custom Objects Schema API
  slug: encharge-customobjectsschema-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/encharge/refs/heads/main/openapi/encharge-customobjectsschema-api-openapi.yml
- filename: encharge-emailtemplates-api-openapi.yml
  format: yaml
  label: Encharge Email Templates API
  slug: encharge-emailtemplates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/encharge/refs/heads/main/openapi/encharge-emailtemplates-api-openapi.yml
- filename: encharge-folders-api-openapi.yml
  format: yaml
  label: Encharge Folders API
  slug: encharge-folders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/encharge/refs/heads/main/openapi/encharge-folders-api-openapi.yml
- filename: encharge-people-api-openapi.yml
  format: yaml
  label: Encharge People API
  slug: encharge-people-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/encharge/refs/heads/main/openapi/encharge-people-api-openapi.yml
- filename: encharge-personfields-api-openapi.yml
  format: yaml
  label: Encharge Person Fields API
  slug: encharge-personfields-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/encharge/refs/heads/main/openapi/encharge-personfields-api-openapi.yml
- filename: encharge-segments-api-openapi.yml
  format: yaml
  label: Encharge Segments API
  slug: encharge-segments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/encharge/refs/heads/main/openapi/encharge-segments-api-openapi.yml
- filename: encharge-settings-api-openapi.yml
  format: yaml
  label: Encharge Email Domain Settings API
  slug: encharge-settings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/encharge/refs/heads/main/openapi/encharge-settings-api-openapi.yml
- filename: encharge-tags-api-openapi.yml
  format: yaml
  label: Encharge Tags API
  slug: encharge-tags-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/encharge/refs/heads/main/openapi/encharge-tags-api-openapi.yml
- filename: encharge-tags-management-api-openapi.yml
  format: yaml
  label: Encharge Tags Management API
  slug: encharge-tags-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/encharge/refs/heads/main/openapi/encharge-tags-management-api-openapi.yml
- filename: encharge-webhooks-api-openapi.yml
  format: yaml
  label: Encharge Webhooks API
  slug: encharge-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/encharge/refs/heads/main/openapi/encharge-webhooks-api-openapi.yml
auth_types:
- apiKey
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Encharge Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Encharge secures its APIs with apiKey and oauth2 across 3 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Encharge
provider_slug: encharge
scheme_count: 3
schemes:
- description: "You can use API key authentication if you are using the API for your Encharge account. If you are building an app for others to use, please use the OAuth2 authentication below. Find your API key from https://app.encharge.io/account/info . \n\n While all operations in the API specify oauth2 security, instead you can use an API key in the header or query string."
  in: header
  name: apiKeyHeader
  parameter: X-Encharge-Token
  sources:
  - openapi/encharge-account-api-openapi.yml
  - openapi/encharge-broadcasts-api-openapi.yml
  - openapi/encharge-customobjects-api-openapi.yml
  - openapi/encharge-customobjectsschema-api-openapi.yml
  - openapi/encharge-emailtemplates-api-openapi.yml
  - openapi/encharge-folders-api-openapi.yml
  - openapi/encharge-people-api-openapi.yml
  - openapi/encharge-personfields-api-openapi.yml
  - openapi/encharge-segments-api-openapi.yml
  - openapi/encharge-settings-api-openapi.yml
  - openapi/encharge-tags-api-openapi.yml
  - openapi/encharge-tags-management-api-openapi.yml
  - openapi/encharge-webhooks-api-openapi.yml
  type: apiKey
- description: "You can use API key authentication if you are using the API for your Encharge account. \n\nIf you are building an app for others to use, please use the OAuth2 authentication below. Find your API key from https://app.encharge.io/account/info \n\n While all operations in the API specify oauth2 security, instead you can use an API key in the header or query string."
  in: query
  name: apiKeyQuery
  parameter: token
  sources:
  - openapi/encharge-account-api-openapi.yml
  - openapi/encharge-broadcasts-api-openapi.yml
  - openapi/encharge-customobjects-api-openapi.yml
  - openapi/encharge-customobjectsschema-api-openapi.yml
  - openapi/encharge-emailtemplates-api-openapi.yml
  - openapi/encharge-folders-api-openapi.yml
  - openapi/encharge-people-api-openapi.yml
  - openapi/encharge-personfields-api-openapi.yml
  - openapi/encharge-segments-api-openapi.yml
  - openapi/encharge-settings-api-openapi.yml
  - openapi/encharge-tags-api-openapi.yml
  - openapi/encharge-tags-management-api-openapi.yml
  - openapi/encharge-webhooks-api-openapi.yml
  type: apiKey
- description: "The Encharge API uses OAuth 2 with the authorization code flow. \n\nGet for your OAuth credentials (Client ID and Client Secret) by filling out [this form](https://research.typeform.com/to/I680YtLA)."
  flows:
  - authorizationUrl: https://api.encharge.io/v1/oauth/authorize
    flow: authorizationCode
    scopes: 0
    tokenUrl: https://api.encharge.io/v1/oauth/token
  name: oauth2
  sources:
  - openapi/encharge-account-api-openapi.yml
  - openapi/encharge-broadcasts-api-openapi.yml
  - openapi/encharge-customobjects-api-openapi.yml
  - openapi/encharge-customobjectsschema-api-openapi.yml
  - openapi/encharge-emailtemplates-api-openapi.yml
  - openapi/encharge-folders-api-openapi.yml
  - openapi/encharge-people-api-openapi.yml
  - openapi/encharge-personfields-api-openapi.yml
  - openapi/encharge-segments-api-openapi.yml
  - openapi/encharge-settings-api-openapi.yml
  - openapi/encharge-tags-api-openapi.yml
  - openapi/encharge-tags-management-api-openapi.yml
  - openapi/encharge-webhooks-api-openapi.yml
  type: oauth2
slug: encharge-authentication
source_filename: encharge-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: searched\ndocs:\n  - https://docs.encharge.io/transactional-email-api/authentication\n  - https://docs.encharge.io/getting-started/connecting-your-app-to-encharge/ingest-api\n  - https://app.encharge.io/account/info\nsearched_notes:\n  api_key:\n    header: X-Encharge-Token\n    query_param: token\n    where_to_get: https://app.encharge.io/account/info\n    scope_of_use: >-\n      One account key authenticates all three Encharge APIs — the REST API, the\n      Transactional Email API (POST /v1/emails/send) and the Ingest API, where\n      the same value is called the \"write key\".\n    credential_in_url: >-\n      Documented CORS workaround for the Ingest API puts the write key in the\n      path: https://ingest.encharge.io/v1/{write-key}. Encharge publishes this\n      as supported; it leaks the credential into logs and referrers.\n  oauth2:\n    intended_for: apps built for other Encharge customers (partner integrations)\n    credential_issuance:\
  \ manual — client id/secret requested through a form, not self-serve\n    scopes_reference: none published; the 8 live scopes were read out of operation-level security (see scopes/encharge-scopes.yml)\n  unauthenticated_operation:\n    - operation: GetAccountInfoByFormId\n      path: /accounts/form/{formId}\n      note: >-\n        The spec describes this as returning non-sensitive account information\n        by form id WITHOUT authentication.\nsource: openapi/encharge-account-api-openapi.yml, openapi/encharge-broadcasts-api-openapi.yml,\n  openapi/encharge-customobjects-api-openapi.yml, openapi/encharge-customobjectsschema-api-openapi.yml,\n  openapi/encharge-emailtemplates-api-openapi.yml, openapi/encharge-folders-api-openapi.yml,\n  openapi/encharge-people-api-openapi.yml, openapi/encharge-personfields-api-openapi.yml, openapi/encharge-segments-api-openapi.yml,\n  openapi/encharge-settings-api-openapi.yml, openapi/encharge-tags-api-openapi.yml, openapi/encharge-tags-management-api-openapi.yml\n\
  \  ...\nsummary:\n  types:\n  - apiKey\n  - oauth2\n  api_key_in:\n  - header\n  - query\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: apiKeyHeader\n  type: apiKey\n  in: header\n  parameter: X-Encharge-Token\n  description: \"You can use API key authentication if you are using the API for your Encharge\\\n    \\ account. If you are building an app for others to use, please use the OAuth2 authentication\\\n    \\ below. Find your API key from https://app.encharge.io/account/info . \\n\\n While all operations\\\n    \\ in the API specify oauth2 security, instead you can use an API key in the header or query\\\n    \\ string.\"\n  sources:\n  - openapi/encharge-account-api-openapi.yml\n  - openapi/encharge-broadcasts-api-openapi.yml\n  - openapi/encharge-customobjects-api-openapi.yml\n  - openapi/encharge-customobjectsschema-api-openapi.yml\n  - openapi/encharge-emailtemplates-api-openapi.yml\n  - openapi/encharge-folders-api-openapi.yml\n  - openapi/encharge-people-api-openapi.yml\n\
  \  - openapi/encharge-personfields-api-openapi.yml\n  - openapi/encharge-segments-api-openapi.yml\n  - openapi/encharge-settings-api-openapi.yml\n  - openapi/encharge-tags-api-openapi.yml\n  - openapi/encharge-tags-management-api-openapi.yml\n  - openapi/encharge-webhooks-api-openapi.yml\n- name: apiKeyQuery\n  type: apiKey\n  in: query\n  parameter: token\n  description: \"You can use API key authentication if you are using the API for your Encharge\\\n    \\ account. \\n\\nIf you are building an app for others to use, please use the OAuth2 authentication\\\n    \\ below. Find your API key from https://app.encharge.io/account/info \\n\\n While all operations\\\n    \\ in the API specify oauth2 security, instead you can use an API key in the header or query\\\n    \\ string.\"\n  sources:\n  - openapi/encharge-account-api-openapi.yml\n  - openapi/encharge-broadcasts-api-openapi.yml\n  - openapi/encharge-customobjects-api-openapi.yml\n  - openapi/encharge-customobjectsschema-api-openapi.yml\n\
  \  - openapi/encharge-emailtemplates-api-openapi.yml\n  - openapi/encharge-folders-api-openapi.yml\n  - openapi/encharge-people-api-openapi.yml\n  - openapi/encharge-personfields-api-openapi.yml\n  - openapi/encharge-segments-api-openapi.yml\n  - openapi/encharge-settings-api-openapi.yml\n  - openapi/encharge-tags-api-openapi.yml\n  - openapi/encharge-tags-management-api-openapi.yml\n  - openapi/encharge-webhooks-api-openapi.yml\n- name: oauth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://api.encharge.io/v1/oauth/authorize\n    tokenUrl: https://api.encharge.io/v1/oauth/token\n    scopes: 0\n  description: \"The Encharge API uses OAuth 2 with the authorization code flow. \\n\\nGet for\\\n    \\ your OAuth credentials (Client ID and Client Secret) by filling out [this form](https://research.typeform.com/to/I680YtLA).\"\n  sources:\n  - openapi/encharge-account-api-openapi.yml\n  - openapi/encharge-broadcasts-api-openapi.yml\n  - openapi/encharge-customobjects-api-openapi.yml\n\
  \  - openapi/encharge-customobjectsschema-api-openapi.yml\n  - openapi/encharge-emailtemplates-api-openapi.yml\n  - openapi/encharge-folders-api-openapi.yml\n  - openapi/encharge-people-api-openapi.yml\n  - openapi/encharge-personfields-api-openapi.yml\n  - openapi/encharge-segments-api-openapi.yml\n  - openapi/encharge-settings-api-openapi.yml\n  - openapi/encharge-tags-api-openapi.yml\n  - openapi/encharge-tags-management-api-openapi.yml\n  - openapi/encharge-webhooks-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/encharge/refs/heads/main/authentication/encharge-authentication.yml
summary_line: apiKey/oauth2 · 3 schemes
tags:
- Email Marketing
- Marketing Automation
- Transactional Email
- Software-as-a-Service
- Behavioral Email
- Customer Engagement
- Customer Data
- Webhook
---
