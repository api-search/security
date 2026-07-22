---
api_key_in: []
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Spredfast Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Spredfast secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Spredfast
provider_slug: spredfast
scheme_count: 1
schemes:
- flows:
  - description: Developer Auth Flow — the app obtains an accessToken via OAuth 2.0 that is then presented on all subsequent Khoros Marketing (Spredfast) API calls.
    flow: authorizationCode
  name: OAuth2
  sources:
  - https://developer.khoros.com/khorosmarketingdevdocs/docs/getting-started-with-the-conversations-api
  type: oauth2
slug: spredfast-authentication
source_filename: spredfast-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://developer.khoros.com/khorosmarketingdevdocs/docs/getting-started-with-the-conversations-api\ndocs: https://developer.khoros.com/khorosmarketingdevdocs\nnote: >-\n  Spredfast's social marketing API is now the Khoros Marketing API family\n  (Conversations, Publishing, Analytics Reporting, Notification, CRM). The\n  developer center documents an OAuth 2.0 developer auth flow: clients complete\n  the auth flow to obtain an accessToken that authenticates all subsequent calls\n  to the Khoros Marketing Conversations API. No OpenAPI/Swagger definition is\n  published, so the scheme below is captured from the docs rather than derived.\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: OAuth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    description: >-\n      Developer Auth Flow — the app obtains an accessToken via OAuth 2.0 that is\n      then presented on all subsequent\
  \ Khoros Marketing (Spredfast) API calls.\n  sources:\n  - https://developer.khoros.com/khorosmarketingdevdocs/docs/getting-started-with-the-conversations-api\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/spredfast/refs/heads/main/authentication/spredfast-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Company
- Social Media
- Social Media Management
- Marketing
- Social Marketing
- Publishing
- Analytics
- Engagement
---
