---
api_key_in: []
api_specs:
- filename: clearslide-insights-api-openapi.yml
  format: yaml
  label: ClearSlide Insights API
  slug: clearslide-insights-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clearslide/refs/heads/main/openapi/clearslide-insights-api-openapi.yml
- filename: clearslide-links-api-openapi.yml
  format: yaml
  label: ClearSlide Links API
  slug: clearslide-links-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clearslide/refs/heads/main/openapi/clearslide-links-api-openapi.yml
- filename: clearslide-meetings-api-openapi.yml
  format: yaml
  label: ClearSlide Meetings API
  slug: clearslide-meetings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clearslide/refs/heads/main/openapi/clearslide-meetings-api-openapi.yml
- filename: clearslide-presentations-api-openapi.yml
  format: yaml
  label: ClearSlide Presentations API
  slug: clearslide-presentations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clearslide/refs/heads/main/openapi/clearslide-presentations-api-openapi.yml
- filename: clearslide-upload-api-openapi.yml
  format: yaml
  label: ClearSlide Upload API
  slug: clearslide-upload-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clearslide/refs/heads/main/openapi/clearslide-upload-api-openapi.yml
- filename: clearslide-users-api-openapi.yml
  format: yaml
  label: ClearSlide Users API
  slug: clearslide-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clearslide/refs/heads/main/openapi/clearslide-users-api-openapi.yml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Clearslide Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- password
overview: ClearSlide secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode and password flow(s).
provider_name: ClearSlide
provider_slug: clearslide
scheme_count: 1
schemes:
- description: ClearSlide supports OAuth 2.0 Authorization Code (RFC 6749 §4.1) and Resource Owner Password Credentials (RFC 6749 §4.3) grants. Register a client redirect URL with apisupport@clearslide.com to receive a client id and client secret.
  flows:
  - authorizationUrl: https://oauth.platform.clearslide.com/oauth/authorize
    flow: authorizationCode
    scopes: 2
    tokenUrl: https://oauth.platform.clearslide.com/oauth/token
  - flow: password
    scopes: 2
    tokenUrl: https://oauth.platform.clearslide.com/oauth/token
  name: oauth2
  sources:
  - openapi/clearslide-openapi.yml
  type: oauth2
slug: clearslide-authentication
source_filename: clearslide-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: openapi/clearslide-openapi.yml\ndocs: https://developer.clearslide.com/docs/oauth-20\nregistration: mailto:apisupport@clearslide.com\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\n  - password\nschemes:\n- name: oauth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://oauth.platform.clearslide.com/oauth/authorize\n    tokenUrl: https://oauth.platform.clearslide.com/oauth/token\n    scopes: 2\n  - flow: password\n    tokenUrl: https://oauth.platform.clearslide.com/oauth/token\n    scopes: 2\n  description: ClearSlide supports OAuth 2.0 Authorization Code (RFC 6749 §4.1) and Resource\n    Owner Password Credentials (RFC 6749 §4.3) grants. Register a client redirect URL with apisupport@clearslide.com\n    to receive a client id and client secret.\n  sources:\n  - openapi/clearslide-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/clearslide/refs/heads/main/authentication/clearslide-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Company
- Sales Engagement
- Sales Enablement
- Content Management
- Presentations
- Analytics
- Meetings
- CRM
- OAuth
- SCIM
---
