---
api_key_in: []
auth_types:
- oauth2
- http
description: ''
kind: authentication
layout: security
method: searched
name: Lithium Technologies Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Lithium Technologies secures its APIs with oauth2 and http across 4 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Lithium Technologies
provider_slug: lithium-technologies
scheme_count: 4
schemes:
- api: Khoros Marketing Conversations API
  base_url: https://api.spredfast.com/v2
  description: '3-legged OAuth 2.0. The documented sequence is a call to `/authorize`, then `/grant`, then `/token`, which returns an `accessToken` presented on subsequent calls as `Authorization: Bearer <accessToken>`.'
  docs: https://developer.khoros.com/khorosmarketingdevdocs/docs/getting-started-with-the-conversations-api
  flow: authorizationCode
  name: MarketingOAuth2
  source: https://developer.khoros.com/khorosmarketingdevdocs/docs/getting-started-with-the-conversations-api
  token_lifetime: 2 years
  token_notes: The access token persists across the user's password changes and can be revoked at any time from Profile Settings.
  type: oauth2
- api: Khoros Care APIs
  description: HTTP Basic authentication via the Authorization header, used for all Khoros Care API calls outside the Automation Framework. Khoros recommends creating a single distinct user account per project.
  docs: https://developer.khoros.com/khoroscaredevdocs/docs/khoros-care-integration-overview
  name: CareBasicAuth
  scheme: basic
  source: https://developer.khoros.com/khoroscaredevdocs/docs/khoros-care-integration-overview
  type: http
- api: Khoros Care APIs
  description: Bearer token used by the Khoros Care Automation Framework. The token is created by a permissioned user with Basic Auth and is refreshable.
  docs: https://developer.khoros.com/khoroscaredevdocs/docs/khoros-care-integration-overview
  name: CareAutomationBearer
  scheme: bearer
  source: https://developer.khoros.com/khoroscaredevdocs/docs/khoros-care-integration-overview
  token_lifetime: 90 days
  type: http
- api: Khoros Communities Aurora GraphQL API
  description: Aurora API credentials are generated through "API Apps" in the community admin. The credential detail page is gated behind the Khoros community login, so the exact header/parameter placement is not recorded here rather than guessed.
  docs: https://developer.khoros.com/khorosauroradevdocs/docs/generating-api-credentials-with-api-apps
  name: AuroraApiApps
  source: https://developer.khoros.com/khorosauroradevdocs/docs/generating-api-credentials-with-api-apps
  status: partial — credential placement not publicly documented
  type: apiKey
slug: lithium-technologies-authentication
source_filename: lithium-technologies-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: https://developer.khoros.com/khorosmarketingdevdocs/docs/getting-started-with-the-conversations-api\ndocs: https://developer.khoros.com/\nnotes: >-\n  Derived-from-OpenAPI was not possible — Khoros publishes no machine-readable OpenAPI. This profile is\n  read directly from the public developer documentation. The five Khoros surfaces do not share one auth\n  model: Marketing is OAuth 2.0, Care is HTTP Basic plus a bearer token, and the Communities surfaces\n  use portal-issued API app credentials.\nsummary:\n  types:\n  - oauth2\n  - http\n  oauth2_flows:\n  - authorizationCode\n  http_schemes:\n  - basic\n  - bearer\n  api_key_in: []\nschemes:\n- name: MarketingOAuth2\n  api: Khoros Marketing Conversations API\n  type: oauth2\n  flow: authorizationCode\n  description: >-\n    3-legged OAuth 2.0. The documented sequence is a call to `/authorize`, then `/grant`, then `/token`,\n    which returns an `accessToken` presented on\
  \ subsequent calls as `Authorization: Bearer <accessToken>`.\n  token_lifetime: 2 years\n  token_notes: >-\n    The access token persists across the user's password changes and can be revoked at any time from\n    Profile Settings.\n  base_url: https://api.spredfast.com/v2\n  docs: https://developer.khoros.com/khorosmarketingdevdocs/docs/getting-started-with-the-conversations-api\n  source: https://developer.khoros.com/khorosmarketingdevdocs/docs/getting-started-with-the-conversations-api\n- name: CareBasicAuth\n  api: Khoros Care APIs\n  type: http\n  scheme: basic\n  description: >-\n    HTTP Basic authentication via the Authorization header, used for all Khoros Care API calls outside\n    the Automation Framework. Khoros recommends creating a single distinct user account per project.\n  docs: https://developer.khoros.com/khoroscaredevdocs/docs/khoros-care-integration-overview\n  source: https://developer.khoros.com/khoroscaredevdocs/docs/khoros-care-integration-overview\n- name: CareAutomationBearer\n\
  \  api: Khoros Care APIs\n  type: http\n  scheme: bearer\n  description: >-\n    Bearer token used by the Khoros Care Automation Framework. The token is created by a permissioned\n    user with Basic Auth and is refreshable.\n  token_lifetime: 90 days\n  docs: https://developer.khoros.com/khoroscaredevdocs/docs/khoros-care-integration-overview\n  source: https://developer.khoros.com/khoroscaredevdocs/docs/khoros-care-integration-overview\n- name: AuroraApiApps\n  api: Khoros Communities Aurora GraphQL API\n  type: apiKey\n  description: >-\n    Aurora API credentials are generated through \"API Apps\" in the community admin. The credential\n    detail page is gated behind the Khoros community login, so the exact header/parameter placement is\n    not recorded here rather than guessed.\n  docs: https://developer.khoros.com/khorosauroradevdocs/docs/generating-api-credentials-with-api-apps\n  source: https://developer.khoros.com/khorosauroradevdocs/docs/generating-api-credentials-with-api-apps\n\
  \  status: partial — credential placement not publicly documented\nscopes: none documented publicly\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/lithium-technologies/refs/heads/main/authentication/lithium-technologies-authentication.yml
summary_line: oauth2/http · 4 schemes
tags:
- Company
- Enterprise Software
- Online Community
- Social Media Management
- Customer Engagement
- Customer Support
- Marketing
- Conversational AI
- Martech
---
