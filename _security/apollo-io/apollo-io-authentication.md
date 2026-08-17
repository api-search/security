---
api_key_in:
- header
api_specs:
- filename: apollo-io-enrichment-api-openapi.yml
  format: yaml
  label: Apollo.io Enrichment API
  slug: apollo-io-enrichment-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apollo-io/refs/heads/main/openapi/apollo-io-enrichment-api-openapi.yml
- filename: apollo-io-search-api-openapi.yml
  format: yaml
  label: Apollo.io Search API
  slug: apollo-io-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apollo-io/refs/heads/main/openapi/apollo-io-search-api-openapi.yml
- filename: apollo-io-accounts-api-openapi.yml
  format: yaml
  label: Apollo.io Accounts API
  slug: apollo-io-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apollo-io/refs/heads/main/openapi/apollo-io-accounts-api-openapi.yml
- filename: apollo-io-contacts-api-openapi.yml
  format: yaml
  label: Apollo.io Contacts API
  slug: apollo-io-contacts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apollo-io/refs/heads/main/openapi/apollo-io-contacts-api-openapi.yml
- filename: apollo-io-deals-api-openapi.yml
  format: yaml
  label: Apollo.io Deals API
  slug: apollo-io-deals-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apollo-io/refs/heads/main/openapi/apollo-io-deals-api-openapi.yml
- filename: apollo-io-sequences-api-openapi.yml
  format: yaml
  label: Apollo.io Sequences API
  slug: apollo-io-sequences-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apollo-io/refs/heads/main/openapi/apollo-io-sequences-api-openapi.yml
- filename: apollo-io-emailer-messages-api-openapi.yml
  format: yaml
  label: Apollo.io Emailer Messages API
  slug: apollo-io-emailer-messages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apollo-io/refs/heads/main/openapi/apollo-io-emailer-messages-api-openapi.yml
- filename: apollo-io-tasks-api-openapi.yml
  format: yaml
  label: Apollo.io Tasks API
  slug: apollo-io-tasks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apollo-io/refs/heads/main/openapi/apollo-io-tasks-api-openapi.yml
- filename: apollo-io-calls-api-openapi.yml
  format: yaml
  label: Apollo.io Calls API
  slug: apollo-io-calls-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apollo-io/refs/heads/main/openapi/apollo-io-calls-api-openapi.yml
- filename: apollo-io-conversations-api-openapi.yml
  format: yaml
  label: Apollo.io Conversations API
  slug: apollo-io-conversations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apollo-io/refs/heads/main/openapi/apollo-io-conversations-api-openapi.yml
- filename: apollo-io-analytics-api-openapi.yml
  format: yaml
  label: Apollo.io Analytics API
  slug: apollo-io-analytics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apollo-io/refs/heads/main/openapi/apollo-io-analytics-api-openapi.yml
- filename: apollo-io-fields-api-openapi.yml
  format: yaml
  label: Apollo.io Fields API
  slug: apollo-io-fields-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apollo-io/refs/heads/main/openapi/apollo-io-fields-api-openapi.yml
- filename: apollo-io-miscellaneous-api-openapi.yml
  format: yaml
  label: Apollo.io Miscellaneous API
  slug: apollo-io-miscellaneous-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apollo-io/refs/heads/main/openapi/apollo-io-miscellaneous-api-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: derived
name: Apollo Io Authentication
name_suffix: Authentication
oauth_flows: []
overview: Apollo.io secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Apollo.io
provider_slug: apollo-io
scheme_count: 2
schemes:
- description: '[Recommended] API key, passed in the `x-api-key` request header.

    See [Create API Keys](https://docs.apollo.io/docs/create-api-key).'
  in: header
  name: apiKey
  parameter: x-api-key
  sources:
  - openapi/apollo-io-accounts-api-openapi.yml
  - openapi/apollo-io-analytics-api-openapi.yml
  - openapi/apollo-io-calls-api-openapi.yml
  - openapi/apollo-io-contacts-api-openapi.yml
  - openapi/apollo-io-conversations-api-openapi.yml
  - openapi/apollo-io-deals-api-openapi.yml
  - openapi/apollo-io-emailer-messages-api-openapi.yml
  - openapi/apollo-io-enrichment-api-openapi.yml
  - openapi/apollo-io-fields-api-openapi.yml
  - openapi/apollo-io-miscellaneous-api-openapi.yml
  - openapi/apollo-io-search-api-openapi.yml
  - openapi/apollo-io-sequences-api-openapi.yml
  - openapi/apollo-io-tasks-api-openapi.yml
  type: apiKey
- bearerFormat: JWT
  description: 'OAuth 2.0 access token, used by Apollo partners building integrations.

    See the [OAuth 2.0 authorization flow](https://docs.apollo.io/docs/use-oauth-20-authorization-flow-to-access-apollo-user-information-partners).'
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/apollo-io-accounts-api-openapi.yml
  - openapi/apollo-io-analytics-api-openapi.yml
  - openapi/apollo-io-calls-api-openapi.yml
  - openapi/apollo-io-contacts-api-openapi.yml
  - openapi/apollo-io-conversations-api-openapi.yml
  - openapi/apollo-io-deals-api-openapi.yml
  - openapi/apollo-io-emailer-messages-api-openapi.yml
  - openapi/apollo-io-enrichment-api-openapi.yml
  - openapi/apollo-io-fields-api-openapi.yml
  - openapi/apollo-io-miscellaneous-api-openapi.yml
  - openapi/apollo-io-search-api-openapi.yml
  - openapi/apollo-io-sequences-api-openapi.yml
  - openapi/apollo-io-tasks-api-openapi.yml
  type: http
slug: apollo-io-authentication
source_filename: apollo-io-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: derived\nsource: openapi/apollo-io-accounts-api-openapi.yml, openapi/apollo-io-analytics-api-openapi.yml,\n  openapi/apollo-io-calls-api-openapi.yml, openapi/apollo-io-contacts-api-openapi.yml, openapi/apollo-io-conversations-api-openapi.yml,\n  openapi/apollo-io-deals-api-openapi.yml, openapi/apollo-io-emailer-messages-api-openapi.yml,\n  openapi/apollo-io-enrichment-api-openapi.yml, openapi/apollo-io-fields-api-openapi.yml, openapi/apollo-io-miscellaneous-api-openapi.yml,\n  openapi/apollo-io-search-api-openapi.yml, openapi/apollo-io-sequences-api-openapi.yml ...\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: apiKey\n  type: apiKey\n  in: header\n  parameter: x-api-key\n  description: |-\n    [Recommended] API key, passed in the `x-api-key` request header.\n    See [Create API Keys](https://docs.apollo.io/docs/create-api-key).\n  sources:\n  - openapi/apollo-io-accounts-api-openapi.yml\n  - openapi/apollo-io-analytics-api-openapi.yml\n\
  \  - openapi/apollo-io-calls-api-openapi.yml\n  - openapi/apollo-io-contacts-api-openapi.yml\n  - openapi/apollo-io-conversations-api-openapi.yml\n  - openapi/apollo-io-deals-api-openapi.yml\n  - openapi/apollo-io-emailer-messages-api-openapi.yml\n  - openapi/apollo-io-enrichment-api-openapi.yml\n  - openapi/apollo-io-fields-api-openapi.yml\n  - openapi/apollo-io-miscellaneous-api-openapi.yml\n  - openapi/apollo-io-search-api-openapi.yml\n  - openapi/apollo-io-sequences-api-openapi.yml\n  - openapi/apollo-io-tasks-api-openapi.yml\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: |-\n    OAuth 2.0 access token, used by Apollo partners building integrations.\n    See the [OAuth 2.0 authorization flow](https://docs.apollo.io/docs/use-oauth-20-authorization-flow-to-access-apollo-user-information-partners).\n  sources:\n  - openapi/apollo-io-accounts-api-openapi.yml\n  - openapi/apollo-io-analytics-api-openapi.yml\n  - openapi/apollo-io-calls-api-openapi.yml\n\
  \  - openapi/apollo-io-contacts-api-openapi.yml\n  - openapi/apollo-io-conversations-api-openapi.yml\n  - openapi/apollo-io-deals-api-openapi.yml\n  - openapi/apollo-io-emailer-messages-api-openapi.yml\n  - openapi/apollo-io-enrichment-api-openapi.yml\n  - openapi/apollo-io-fields-api-openapi.yml\n  - openapi/apollo-io-miscellaneous-api-openapi.yml\n  - openapi/apollo-io-search-api-openapi.yml\n  - openapi/apollo-io-sequences-api-openapi.yml\n  - openapi/apollo-io-tasks-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/apollo-io/refs/heads/main/authentication/apollo-io-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Sales Intelligence
- Prospecting
- Engagement
- B2B Data
- Enrichment
- CRM
- Sales Engagement
- Conversation Intelligence
- MCP
- SaaS
---
