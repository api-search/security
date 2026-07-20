---
api_key_in: []
api_specs:
- filename: lithium-care-conversation-api-v2-openapi.json
  format: json
  label: Khoros Care API
  slug: care
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lithium/refs/heads/main/openapi/lithium-care-conversation-api-v2-openapi.json
- filename: lithium-marketing-conversations-openapi.json
  format: json
  label: Khoros Marketing API
  slug: marketing
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lithium/refs/heads/main/openapi/lithium-marketing-conversations-openapi.json
- filename: lithium-flow-flow-rest-api-openapi.json
  format: json
  label: Khoros Flow API
  slug: flow
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lithium/refs/heads/main/openapi/lithium-flow-flow-rest-api-openapi.json
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Lithium Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- clientCredentials
overview: Lithium secures its APIs with http and oauth2 across 3 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode and clientCredentials flow(s).
provider_name: Lithium
provider_slug: lithium
scheme_count: 3
schemes:
- name: sec0
  scheme: basic
  sources:
  - openapi/lithium-care-analytics-reports-openapi.json
  - openapi/lithium-care-conversation-tag-rules-v2-openapi.json
  - openapi/lithium-care-secure-forms-api-v2-openapi.json
  - openapi/lithium-care-supervisor-reports-api-openapi.json
  type: http
- flows:
  - flow: clientCredentials
    scopes: 0
    tokenUrl: https://example.com/oauth2/token
  name: sec0
  sources:
  - openapi/lithium-marketing-beta-analytics-api-openapi.json
  - openapi/lithium-marketing-conversations-openapi.json
  - openapi/lithium-marketing-crm-openapi.json
  - openapi/lithium-marketing-introspection-api-openapi.json
  - openapi/lithium-marketing-labelsets-api-openapi.json
  - openapi/lithium-marketing-notification-service-openapi.json
  - openapi/lithium-marketing-stream-api-openapi.json
  type: oauth2
- flows:
  - authorizationUrl: https://login.spredfast.com/v3/oauth/authorize
    flow: authorizationCode
    scopes: 1
    tokenUrl: https://login.spredfast.com/v3/oauth/token
  name: oauth2
  sources:
  - openapi/lithium-marketing-conversations-api-v1-openapi.json
  type: oauth2
slug: lithium-authentication
source_filename: lithium-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: openapi/lithium-care-analytics-reports-openapi.json, openapi/lithium-care-conversation-tag-rules-v2-openapi.json,\n  openapi/lithium-care-secure-forms-api-v2-openapi.json, openapi/lithium-care-supervisor-reports-api-openapi.json,\n  openapi/lithium-marketing-beta-analytics-api-openapi.json, openapi/lithium-marketing-conversations-api-v1-openapi.json,\n  openapi/lithium-marketing-conversations-openapi.json, openapi/lithium-marketing-crm-openapi.json,\n  openapi/lithium-marketing-introspection-api-openapi.json, openapi/lithium-marketing-labelsets-api-openapi.json,\n  openapi/lithium-marketing-notification-service-openapi.json, openapi/lithium-marketing-stream-api-openapi.json\nsummary:\n  types:\n  - http\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\n  - clientCredentials\nschemes:\n- name: sec0\n  type: http\n  scheme: basic\n  sources:\n  - openapi/lithium-care-analytics-reports-openapi.json\n  - openapi/lithium-care-conversation-tag-rules-v2-openapi.json\n\
  \  - openapi/lithium-care-secure-forms-api-v2-openapi.json\n  - openapi/lithium-care-supervisor-reports-api-openapi.json\n- name: sec0\n  type: oauth2\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://example.com/oauth2/token\n    scopes: 0\n  sources:\n  - openapi/lithium-marketing-beta-analytics-api-openapi.json\n  - openapi/lithium-marketing-conversations-openapi.json\n  - openapi/lithium-marketing-crm-openapi.json\n  - openapi/lithium-marketing-introspection-api-openapi.json\n  - openapi/lithium-marketing-labelsets-api-openapi.json\n  - openapi/lithium-marketing-notification-service-openapi.json\n  - openapi/lithium-marketing-stream-api-openapi.json\n- name: oauth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://login.spredfast.com/v3/oauth/authorize\n    tokenUrl: https://login.spredfast.com/v3/oauth/token\n    scopes: 1\n  sources:\n  - openapi/lithium-marketing-conversations-api-v1-openapi.json\n\ndocs:\n  care_jwt: https://developer.khoros.com/khoroscaredevdocs/docs/jwt-authentication\n\
  \  care_overview: https://developer.khoros.com/khoroscaredevdocs/docs/khoros-care-integration-overview\n  community_api_apps: https://developer.khoros.com/khorosauroradevdocs/docs/generating-api-credentials-with-api-apps\n  marketing_events_auth: https://developer.khoros.com/khorosmarketingdevdocs/docs/events-authentication\n\ndocumented_models:\n  - product: Khoros Care\n    schemes: [http-basic, jwt]\n    detail: >-\n      Care v1 and v2 APIs use HTTP Basic against the per-instance\n      {instance}.response.lithium.com host. The Automation Framework's Bot API v3 on\n      api.app.lithium.com uses a signed JSON Web Token (header/payload/signature) instead —\n      the documentation is explicit that only Bot API v3 uses JWT. The Care Authentication\n      API v2 (/api/v2/tokens) exchanges credentials for a token.\n    docs: https://developer.khoros.com/khoroscaredevdocs/docs/jwt-authentication\n  - product: Khoros Marketing\n    schemes: [oauth2]\n    detail: >-\n      OAuth 2.0 against\
  \ login.spredfast.com. Token introspection is available at\n      https://api.spredfast.com/v2/whoami. Tenancy is carried in x-sf-company-id /\n      x-sf-initiative / x-sf-user-email request headers alongside the token.\n  - product: Khoros Community\n    schemes: [session, api-app-credentials]\n    detail: >-\n      Community v2 rejects anonymous calls with its JSON error envelope (code 203).\n      Credentials are provisioned as API apps through the community admin. Documentation is\n      behind the Atlas login.\n  - product: Khoros Flow\n    schemes: [api-key]\n    detail: Token-based access to the flow.ai REST API.\n\ncaveats:\n  - >-\n    The `sec0` clientCredentials scheme repeated across seven Khoros Marketing definitions\n    declares tokenUrl https://example.com/oauth2/token with an empty scopes map. That is a\n    ReadMe API-designer placeholder, not a real authorization server — the working OAuth\n    endpoints are the login.spredfast.com pair on the Conversations API v1 definition.\n\
  \  - >-\n    Only 12 of the 28 harvested definitions declare any security scheme at all; the\n    remaining 16 (mostly the per-instance Care v2 APIs) document authentication in prose\n    only.\n\nrelated:\n  scopes: ../scopes/lithium-scopes.yml\n  conventions: ../conventions/lithium-conventions.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/lithium/refs/heads/main/authentication/lithium-authentication.yml
summary_line: http/oauth2 · 3 schemes
tags:
- Company
- Martech
- Community
- Social Media
- Customer Engagement
- Customer Support
- Chatbots
- Messaging
- Analytics
- Marketing
---
