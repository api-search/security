---
api_key_in: []
api_specs:
- filename: google-search-console-search-analytics-api-openapi.yml
  format: yaml
  label: Google Search Console Search Analytics API
  slug: google-search-console-search-analytics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/google-search-console/refs/heads/main/openapi/google-search-console-search-analytics-api-openapi.yml
- filename: google-search-console-sitemaps-api-openapi.yml
  format: yaml
  label: Google Search Console Sitemaps API
  slug: google-search-console-sitemaps-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/google-search-console/refs/heads/main/openapi/google-search-console-sitemaps-api-openapi.yml
- filename: google-search-console-sites-api-openapi.yml
  format: yaml
  label: Google Search Console Sites API
  slug: google-search-console-sites-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/google-search-console/refs/heads/main/openapi/google-search-console-sites-api-openapi.yml
- filename: google-search-console-url-inspection-api-openapi.yml
  format: yaml
  label: Google Search Console URL Inspection API
  slug: google-search-console-url-inspection-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/google-search-console/refs/heads/main/openapi/google-search-console-url-inspection-api-openapi.yml
- filename: google-search-console-urlnotifications-api-openapi.yml
  format: yaml
  label: Google Search Console URL Notifications API
  slug: google-search-console-urlnotifications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/google-search-console/refs/heads/main/openapi/google-search-console-urlnotifications-api-openapi.yml
- filename: google-search-console-urltestingtools-api-openapi.yml
  format: yaml
  label: Google Search Console URL Testing Tools API
  slug: google-search-console-urltestingtools-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/google-search-console/refs/heads/main/openapi/google-search-console-urltestingtools-api-openapi.yml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Google Search Console Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Google Search Console secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Google Search Console
provider_slug: google-search-console
scheme_count: 1
schemes:
- description: 'Google OAuth 2.0. Authorization server metadata: https://accounts.google.com/.well-known/openid-configuration'
  flows:
  - authorizationUrl: https://accounts.google.com/o/oauth2/v2/auth
    flow: authorizationCode
    scopes: 1
    tokenUrl: https://oauth2.googleapis.com/token
  name: OAuth2
  sources:
  - openapi/google-search-console-indexing-api-openapi.yml
  - openapi/google-search-console-search-analytics-api-openapi.yml
  - openapi/google-search-console-sitemaps-api-openapi.yml
  - openapi/google-search-console-sites-api-openapi.yml
  - openapi/google-search-console-url-inspection-api-openapi.yml
  - openapi/google-search-console-url-testing-tools-api-openapi.yml
  type: oauth2
slug: google-search-console-authentication
source_filename: google-search-console-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: searched\ndocs: https://developers.google.com/webmaster-tools/v1/how-tos/authorizing\nsource: >-\n  Confirmed against the provider's authorization how-to and against the OAuth 2.0 authorization\n  server metadata probed live on 2026-08-13 at\n  https://accounts.google.com/.well-known/openid-configuration (HTTP 200). Baseline derived from\n  openapi/google-search-console-indexing-api-openapi.yml, openapi/google-search-console-search-analytics-api-openapi.yml,\n  openapi/google-search-console-sitemaps-api-openapi.yml, openapi/google-search-console-sites-api-openapi.yml,\n  openapi/google-search-console-url-inspection-api-openapi.yml, openapi/google-search-console-url-testing-tools-api-openapi.yml\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: OAuth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://accounts.google.com/o/oauth2/v2/auth\n    tokenUrl: https://oauth2.googleapis.com/token\n\
  \    scopes: 1\n  description: 'Google OAuth 2.0. Authorization server metadata: https://accounts.google.com/.well-known/openid-configuration'\n  sources:\n  - openapi/google-search-console-indexing-api-openapi.yml\n  - openapi/google-search-console-search-analytics-api-openapi.yml\n  - openapi/google-search-console-sitemaps-api-openapi.yml\n  - openapi/google-search-console-sites-api-openapi.yml\n  - openapi/google-search-console-url-inspection-api-openapi.yml\n  - openapi/google-search-console-url-testing-tools-api-openapi.yml\nauthorization_server:\n  issuer: https://accounts.google.com\n  metadata: https://accounts.google.com/.well-known/openid-configuration\n  server_metadata: https://accounts.google.com/.well-known/oauth-authorization-server\n  saved:\n  - well-known/google-search-console-openid-configuration.json\n  - well-known/google-search-console-oauth-authorization-server.json\n  grant_types_supported:\n  - authorization_code\n  - refresh_token\n  - urn:ietf:params:oauth:grant-type:device_code\n\
  \  - urn:ietf:params:oauth:grant-type:jwt-bearer\nscopes:\n- https://www.googleapis.com/auth/webmasters\n- https://www.googleapis.com/auth/webmasters.readonly\n- https://www.googleapis.com/auth/indexing\nidentities:\n- type: user\n  note: Authorization code flow with offline access for a refresh token.\n- type: service account\n  note: >-\n    JWT bearer grant. The standard pattern for server-side integrations and the required one for\n    the Indexing API, where the service account must additionally be added as an Owner of the\n    Search Console property.\napi_key:\n  supported: partial\n  note: >-\n    The Google API front end accepts a `key` query parameter for project identification, but no\n    Search Console operation that reads or writes site data is authorized by an API key alone.\nnotes:\n- >-\n  Authorization is per verified property, not per Cloud project. A valid token with the right scope\n  still returns 403 insufficientPermissions if the account does not own the property\
  \ or the siteUrl\n  string does not match it exactly.\nmaintainers:\n- FN: Kin Lane\n  email: kin@apievangelist.com\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/google-search-console/refs/heads/main/authentication/google-search-console-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Analytics
- Google
- Indexing
- Search
- Search Analytics
- SEO
- Sitemap
- URL Inspection
- Webmaster Tools
---
