---
api_key_in:
- header
api_specs:
- filename: apollo-api-documentation-accounts-api-openapi.yml
  format: yaml
  label: Apollo API Accounts
  slug: apollo-api-documentation-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apollo-api-documentation/refs/heads/main/openapi/apollo-api-documentation-accounts-api-openapi.yml
- filename: apollo-api-documentation-analytics-api-openapi.yml
  format: yaml
  label: Apollo API Analytics
  slug: apollo-api-documentation-analytics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apollo-api-documentation/refs/heads/main/openapi/apollo-api-documentation-analytics-api-openapi.yml
- filename: apollo-api-documentation-calls-api-openapi.yml
  format: yaml
  label: Apollo API Calls
  slug: apollo-api-documentation-calls-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apollo-api-documentation/refs/heads/main/openapi/apollo-api-documentation-calls-api-openapi.yml
- filename: apollo-api-documentation-contacts-api-openapi.yml
  format: yaml
  label: Apollo API Contacts
  slug: apollo-api-documentation-contacts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apollo-api-documentation/refs/heads/main/openapi/apollo-api-documentation-contacts-api-openapi.yml
- filename: apollo-api-documentation-conversations-api-openapi.yml
  format: yaml
  label: Apollo API Conversations
  slug: apollo-api-documentation-conversations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apollo-api-documentation/refs/heads/main/openapi/apollo-api-documentation-conversations-api-openapi.yml
- filename: apollo-api-documentation-deals-api-openapi.yml
  format: yaml
  label: Apollo API Deals
  slug: apollo-api-documentation-deals-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apollo-api-documentation/refs/heads/main/openapi/apollo-api-documentation-deals-api-openapi.yml
- filename: apollo-api-documentation-emailer-messages-api-openapi.yml
  format: yaml
  label: Apollo API Emailer Messages
  slug: apollo-api-documentation-emailer-messages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apollo-api-documentation/refs/heads/main/openapi/apollo-api-documentation-emailer-messages-api-openapi.yml
- filename: apollo-api-documentation-enrichment-api-openapi.yml
  format: yaml
  label: Apollo API Enrichment
  slug: apollo-api-documentation-enrichment-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apollo-api-documentation/refs/heads/main/openapi/apollo-api-documentation-enrichment-api-openapi.yml
- filename: apollo-api-documentation-fields-api-openapi.yml
  format: yaml
  label: Apollo API Fields
  slug: apollo-api-documentation-fields-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apollo-api-documentation/refs/heads/main/openapi/apollo-api-documentation-fields-api-openapi.yml
- filename: apollo-api-documentation-miscellaneous-api-openapi.yml
  format: yaml
  label: Apollo API Miscellaneous
  slug: apollo-api-documentation-miscellaneous-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apollo-api-documentation/refs/heads/main/openapi/apollo-api-documentation-miscellaneous-api-openapi.yml
- filename: apollo-api-documentation-search-api-openapi.yml
  format: yaml
  label: Apollo API Search
  slug: apollo-api-documentation-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apollo-api-documentation/refs/heads/main/openapi/apollo-api-documentation-search-api-openapi.yml
- filename: apollo-api-documentation-sequences-api-openapi.yml
  format: yaml
  label: Apollo API Sequences
  slug: apollo-api-documentation-sequences-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apollo-api-documentation/refs/heads/main/openapi/apollo-api-documentation-sequences-api-openapi.yml
- filename: apollo-api-documentation-tasks-api-openapi.yml
  format: yaml
  label: Apollo API Tasks
  slug: apollo-api-documentation-tasks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apollo-api-documentation/refs/heads/main/openapi/apollo-api-documentation-tasks-api-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: derived
name: Apollo Api Documentation Authentication
name_suffix: Authentication
oauth_flows: []
overview: Apollo API Documentation secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Apollo API Documentation
provider_slug: apollo-api-documentation
scheme_count: 2
schemes:
- description: '[Recommended] API key, passed in the `x-api-key` request header.

    See [Create API Keys](https://docs.apollo.io/docs/create-api-key).'
  in: header
  name: apiKey
  parameter: x-api-key
  sources:
  - openapi/apollo-api-documentation-accounts-api-openapi.yml
  - openapi/apollo-api-documentation-analytics-api-openapi.yml
  - openapi/apollo-api-documentation-calls-api-openapi.yml
  - openapi/apollo-api-documentation-contacts-api-openapi.yml
  - openapi/apollo-api-documentation-conversations-api-openapi.yml
  - openapi/apollo-api-documentation-deals-api-openapi.yml
  - openapi/apollo-api-documentation-emailer-messages-api-openapi.yml
  - openapi/apollo-api-documentation-enrichment-api-openapi.yml
  - openapi/apollo-api-documentation-fields-api-openapi.yml
  - openapi/apollo-api-documentation-miscellaneous-api-openapi.yml
  - openapi/apollo-api-documentation-search-api-openapi.yml
  - openapi/apollo-api-documentation-sequences-api-openapi.yml
  - openapi/apollo-api-documentation-tasks-api-openapi.yml
  type: apiKey
- bearerFormat: JWT
  description: 'OAuth 2.0 access token, used by Apollo partners building integrations.

    See the [OAuth 2.0 authorization flow](https://docs.apollo.io/docs/use-oauth-20-authorization-flow-to-access-apollo-user-information-partners).'
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/apollo-api-documentation-accounts-api-openapi.yml
  - openapi/apollo-api-documentation-analytics-api-openapi.yml
  - openapi/apollo-api-documentation-calls-api-openapi.yml
  - openapi/apollo-api-documentation-contacts-api-openapi.yml
  - openapi/apollo-api-documentation-conversations-api-openapi.yml
  - openapi/apollo-api-documentation-deals-api-openapi.yml
  - openapi/apollo-api-documentation-emailer-messages-api-openapi.yml
  - openapi/apollo-api-documentation-enrichment-api-openapi.yml
  - openapi/apollo-api-documentation-fields-api-openapi.yml
  - openapi/apollo-api-documentation-miscellaneous-api-openapi.yml
  - openapi/apollo-api-documentation-search-api-openapi.yml
  - openapi/apollo-api-documentation-sequences-api-openapi.yml
  - openapi/apollo-api-documentation-tasks-api-openapi.yml
  type: http
slug: apollo-api-documentation-authentication
source_filename: apollo-api-documentation-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-14'\nmethod: derived\nsource: openapi/apollo-api-documentation-accounts-api-openapi.yml, openapi/apollo-api-documentation-analytics-api-openapi.yml,\n  openapi/apollo-api-documentation-calls-api-openapi.yml, openapi/apollo-api-documentation-contacts-api-openapi.yml,\n  openapi/apollo-api-documentation-conversations-api-openapi.yml, openapi/apollo-api-documentation-deals-api-openapi.yml,\n  openapi/apollo-api-documentation-emailer-messages-api-openapi.yml, openapi/apollo-api-documentation-enrichment-api-openapi.yml,\n  openapi/apollo-api-documentation-fields-api-openapi.yml, openapi/apollo-api-documentation-miscellaneous-api-openapi.yml,\n  openapi/apollo-api-documentation-search-api-openapi.yml, openapi/apollo-api-documentation-sequences-api-openapi.yml\n  ...\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: apiKey\n  type: apiKey\n  in: header\n  parameter: x-api-key\n  description: |-\n    [Recommended] API key, passed\
  \ in the `x-api-key` request header.\n    See [Create API Keys](https://docs.apollo.io/docs/create-api-key).\n  sources:\n  - openapi/apollo-api-documentation-accounts-api-openapi.yml\n  - openapi/apollo-api-documentation-analytics-api-openapi.yml\n  - openapi/apollo-api-documentation-calls-api-openapi.yml\n  - openapi/apollo-api-documentation-contacts-api-openapi.yml\n  - openapi/apollo-api-documentation-conversations-api-openapi.yml\n  - openapi/apollo-api-documentation-deals-api-openapi.yml\n  - openapi/apollo-api-documentation-emailer-messages-api-openapi.yml\n  - openapi/apollo-api-documentation-enrichment-api-openapi.yml\n  - openapi/apollo-api-documentation-fields-api-openapi.yml\n  - openapi/apollo-api-documentation-miscellaneous-api-openapi.yml\n  - openapi/apollo-api-documentation-search-api-openapi.yml\n  - openapi/apollo-api-documentation-sequences-api-openapi.yml\n  - openapi/apollo-api-documentation-tasks-api-openapi.yml\n- name: bearerAuth\n  type: http\n  scheme: bearer\n\
  \  bearerFormat: JWT\n  description: |-\n    OAuth 2.0 access token, used by Apollo partners building integrations.\n    See the [OAuth 2.0 authorization flow](https://docs.apollo.io/docs/use-oauth-20-authorization-flow-to-access-apollo-user-information-partners).\n  sources:\n  - openapi/apollo-api-documentation-accounts-api-openapi.yml\n  - openapi/apollo-api-documentation-analytics-api-openapi.yml\n  - openapi/apollo-api-documentation-calls-api-openapi.yml\n  - openapi/apollo-api-documentation-contacts-api-openapi.yml\n  - openapi/apollo-api-documentation-conversations-api-openapi.yml\n  - openapi/apollo-api-documentation-deals-api-openapi.yml\n  - openapi/apollo-api-documentation-emailer-messages-api-openapi.yml\n  - openapi/apollo-api-documentation-enrichment-api-openapi.yml\n  - openapi/apollo-api-documentation-fields-api-openapi.yml\n  - openapi/apollo-api-documentation-miscellaneous-api-openapi.yml\n  - openapi/apollo-api-documentation-search-api-openapi.yml\n  - openapi/apollo-api-documentation-sequences-api-openapi.yml\n\
  \  - openapi/apollo-api-documentation-tasks-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/apollo-api-documentation/refs/heads/main/authentication/apollo-api-documentation-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- API Documentation
- Sales Intelligence
- Data Enrichment
- People Search
- Company Search
- Sales Engagement
- CRM
- MCP
- Agents
- Go-To-Market
---
