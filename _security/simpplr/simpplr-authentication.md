---
anonymous_access: false
api_key_in: []
api_specs:
- filename: simpplr-alerts-api-openapi.yml
  format: yaml
  label: Simpplr Alerts API
  slug: simpplr-alerts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/simpplr/refs/heads/main/openapi/simpplr-alerts-api-openapi.yml
- filename: simpplr-analytics-api-openapi.yml
  format: yaml
  label: Simpplr Analytics API
  slug: simpplr-analytics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/simpplr/refs/heads/main/openapi/simpplr-analytics-api-openapi.yml
- filename: simpplr-audience-api-openapi.yml
  format: yaml
  label: Simpplr Audience API
  slug: simpplr-audience-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/simpplr/refs/heads/main/openapi/simpplr-audience-api-openapi.yml
- filename: simpplr-blogs-api-openapi.yml
  format: yaml
  label: Simpplr Blogs API
  slug: simpplr-blogs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/simpplr/refs/heads/main/openapi/simpplr-blogs-api-openapi.yml
- filename: simpplr-carousels-api-openapi.yml
  format: yaml
  label: Simpplr Carousels API
  slug: simpplr-carousels-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/simpplr/refs/heads/main/openapi/simpplr-carousels-api-openapi.yml
- filename: simpplr-contents-api-openapi.yml
  format: yaml
  label: Simpplr Contents API
  slug: simpplr-contents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/simpplr/refs/heads/main/openapi/simpplr-contents-api-openapi.yml
- filename: simpplr-notifications-api-openapi.yml
  format: yaml
  label: Simpplr Notifications API
  slug: simpplr-notifications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/simpplr/refs/heads/main/openapi/simpplr-notifications-api-openapi.yml
- filename: simpplr-people-api-openapi.yml
  format: yaml
  label: Simpplr People API
  slug: simpplr-people-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/simpplr/refs/heads/main/openapi/simpplr-people-api-openapi.yml
- filename: simpplr-search-api-openapi.yml
  format: yaml
  label: Simpplr Search API
  slug: simpplr-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/simpplr/refs/heads/main/openapi/simpplr-search-api-openapi.yml
- filename: simpplr-simpplr-api-gw-search-people-by-id-api-openapi.yml
  format: yaml
  label: Simpplr Simpplr Api Gw Search People By Id API
  slug: simpplr-simpplr-api-gw-search-people-by-id-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/simpplr/refs/heads/main/openapi/simpplr-simpplr-api-gw-search-people-by-id-api-openapi.yml
- filename: simpplr-sites-api-openapi.yml
  format: yaml
  label: Simpplr Sites API
  slug: simpplr-sites-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/simpplr/refs/heads/main/openapi/simpplr-sites-api-openapi.yml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Simpplr Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: Simpplr secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: Simpplr
provider_slug: simpplr
scheme_count: 1
schemes:
- description: 'The Simpplr Extensibility Center API authenticates external applications with OAuth 2.0 bearer tokens. Simpplr is built on the Salesforce platform, so access is granted by creating and configuring a Salesforce connected app for the Simpplr org; the connected app''s client credentials are exchanged for an OAuth access token that is then sent as an Authorization: Bearer <token> header on every API request. The OpenAPI security scheme exposed in the reference is an oauth2 scheme (sec0).'
  name: OAuth2
  server: https://api.ec.simpplr.com/api
  sources:
  - developer.simpplr.com reference (sec0 oauth2 security scheme)
  type: oauth2
slug: simpplr-authentication
source_filename: simpplr-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://developer.simpplr.com/reference/authenticating-via-an-external-application\ndocs: https://developer.simpplr.com/reference/authenticating-via-an-external-application\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - clientCredentials\n  token_type: bearer\n  platform: salesforce-connected-app\nschemes:\n- name: OAuth2\n  type: oauth2\n  description: >-\n    The Simpplr Extensibility Center API authenticates external applications with\n    OAuth 2.0 bearer tokens. Simpplr is built on the Salesforce platform, so access\n    is granted by creating and configuring a Salesforce connected app for the\n    Simpplr org; the connected app's client credentials are exchanged for an OAuth\n    access token that is then sent as an Authorization: Bearer <token> header on\n    every API request. The OpenAPI security scheme exposed in the reference is an\n    oauth2 scheme (sec0).\n  server: https://api.ec.simpplr.com/api\n  sources:\n\
  \  - developer.simpplr.com reference (sec0 oauth2 security scheme)\nsetup_docs:\n- title: Authenticating via an external application\n  url: https://developer.simpplr.com/reference/authenticating-via-an-external-application\n- title: Creating & configuring a connected app in Salesforce\n  url: https://developer.simpplr.com/reference/creating-configuring-a-connected-app-in-salesforce\nnotes: >-\n  Exact authorization/token URLs are not published verbatim in the OpenAPI (the\n  reference shows placeholder flow URLs); tokens are minted through the Salesforce\n  connected-app OAuth flow documented in the setup pages above.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/simpplr/refs/heads/main/authentication/simpplr-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Company
- Employee Experience
- Intranet
- Employee Communications
- Digital Workplace
- Internal Communications
- Human Resources
- Collaboration
- Enterprise Software
- Salesforce
---
