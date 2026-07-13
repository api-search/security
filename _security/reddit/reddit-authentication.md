---
api_key_in: []
api_specs:
- filename: reddit-data-api-openapi.yml
  format: yaml
  label: Reddit Data API
  slug: data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/reddit/refs/heads/main/openapi/reddit-data-api-openapi.yml
- filename: reddit-ads-api-openapi.yml
  format: yaml
  label: Reddit Ads API
  slug: ads-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/reddit/refs/heads/main/openapi/reddit-ads-api-openapi.yml
- filename: reddit-embeds-openapi.yml
  format: yaml
  label: Reddit Embeds (oEmbed)
  slug: embeds
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/reddit/refs/heads/main/openapi/reddit-embeds-openapi.yml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Reddit Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Reddit secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Reddit
provider_slug: reddit
scheme_count: 1
schemes:
- description: Reddit Ads API uses OAuth 2.0 for authentication. Access tokens are obtained via the authorization code flow.
  flows:
  - authorizationUrl: https://www.reddit.com/api/v1/authorize
    flow: authorizationCode
    scopes: 1
    tokenUrl: https://www.reddit.com/api/v1/access_token
  name: oauth2
  sources:
  - openapi/reddit-ads-api-openapi.yml
  - openapi/reddit-data-api-openapi.yml
  type: oauth2
slug: reddit-authentication
source_filename: reddit-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/reddit-ads-api-openapi.yml, openapi/reddit-data-api-openapi.yml\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: oauth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://www.reddit.com/api/v1/authorize\n    tokenUrl: https://www.reddit.com/api/v1/access_token\n    scopes: 1\n  description: Reddit Ads API uses OAuth 2.0 for authentication. Access tokens are obtained\n    via the authorization code flow.\n  sources:\n  - openapi/reddit-ads-api-openapi.yml\n  - openapi/reddit-data-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/reddit/refs/heads/main/authentication/reddit-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Advertising
- Communities
- Content
- Social Media
- Social News
---
