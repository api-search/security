---
api_key_in: []
api_specs:
- filename: google-admob-accounts-api-openapi.yml
  format: yaml
  label: Google AdMob Accounts API
  slug: google-admob-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/google-admob/refs/heads/main/openapi/google-admob-accounts-api-openapi.yml
- filename: google-admob-adapters-api-openapi.yml
  format: yaml
  label: Google AdMob Adapters API
  slug: google-admob-adapters-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/google-admob/refs/heads/main/openapi/google-admob-adapters-api-openapi.yml
- filename: google-admob-adsources-api-openapi.yml
  format: yaml
  label: Google AdMob Ad Sources API
  slug: google-admob-adsources-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/google-admob/refs/heads/main/openapi/google-admob-adsources-api-openapi.yml
- filename: google-admob-adunitmappings-api-openapi.yml
  format: yaml
  label: Google AdMob Ad Unit Mappings API
  slug: google-admob-adunitmappings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/google-admob/refs/heads/main/openapi/google-admob-adunitmappings-api-openapi.yml
- filename: google-admob-adunits-api-openapi.yml
  format: yaml
  label: Google AdMob Ad Units API
  slug: google-admob-adunits-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/google-admob/refs/heads/main/openapi/google-admob-adunits-api-openapi.yml
- filename: google-admob-apps-api-openapi.yml
  format: yaml
  label: Google AdMob Apps API
  slug: google-admob-apps-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/google-admob/refs/heads/main/openapi/google-admob-apps-api-openapi.yml
- filename: google-admob-campaignreport-api-openapi.yml
  format: yaml
  label: Google AdMob Campaign Report API
  slug: google-admob-campaignreport-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/google-admob/refs/heads/main/openapi/google-admob-campaignreport-api-openapi.yml
- filename: google-admob-mediationabexperiments-api-openapi.yml
  format: yaml
  label: Google AdMob Mediation Ab Experiments API
  slug: google-admob-mediationabexperiments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/google-admob/refs/heads/main/openapi/google-admob-mediationabexperiments-api-openapi.yml
- filename: google-admob-mediationgroups-api-openapi.yml
  format: yaml
  label: Google AdMob Mediation Groups API
  slug: google-admob-mediationgroups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/google-admob/refs/heads/main/openapi/google-admob-mediationgroups-api-openapi.yml
- filename: google-admob-mediationreport-api-openapi.yml
  format: yaml
  label: Google AdMob Mediation Report API
  slug: google-admob-mediationreport-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/google-admob/refs/heads/main/openapi/google-admob-mediationreport-api-openapi.yml
- filename: google-admob-networkreport-api-openapi.yml
  format: yaml
  label: Google AdMob Network Report API
  slug: google-admob-networkreport-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/google-admob/refs/heads/main/openapi/google-admob-networkreport-api-openapi.yml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Google Admob Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Google AdMob secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Google AdMob
provider_slug: google-admob
scheme_count: 1
schemes:
- description: Google OAuth 2.0 user authorization. AdMob does not support service accounts.
  flows:
  - authorizationUrl: https://accounts.google.com/o/oauth2/v2/auth
    flow: authorizationCode
    scopes: 2
    tokenUrl: https://oauth2.googleapis.com/token
  name: GoogleOAuth2
  sources:
  - openapi/google-admob-api-v1-openapi.yml
  - openapi/google-admob-api-v1beta-openapi.yml
  type: oauth2
slug: google-admob-authentication
source_filename: google-admob-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: searched\nsource: openapi/google-admob-api-v1-openapi.yml, openapi/google-admob-api-v1beta-openapi.yml\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: GoogleOAuth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://accounts.google.com/o/oauth2/v2/auth\n    tokenUrl: https://oauth2.googleapis.com/token\n    scopes: 2\n  description: Google OAuth 2.0 user authorization. AdMob does not support service accounts.\n  sources:\n  - openapi/google-admob-api-v1-openapi.yml\n  - openapi/google-admob-api-v1beta-openapi.yml\ndocs: https://developers.google.com/admob/api/v1/getting-started\nsearched_source: https://developers.google.com/admob/api/v1/getting-started\nnotes: 'Upgraded from the mechanically derived profile on 2026-08-13 by reading Google''s own AdMob auth\n  documentation. AdMob accepts ONLY a Google OAuth 2.0 user access token, sent as ''Authorization: Bearer\n \
  \ <token>''. There is no API key, no basic auth, no mutual TLS client auth and - critically for automation\n  - NO SERVICE ACCOUNT SUPPORT, so an unattended agent cannot self-authorize; a human must complete consent\n  and the refresh token must be held. The AdMob API must additionally be enabled on the Google Cloud project\n  behind the OAuth client or every call returns 403 PERMISSION_DENIED. The authorization server is accounts.google.com,\n  whose RFC 8414 metadata and OIDC discovery documents were probed live (both HTTP 200) and saved to well-known/.'\nservice_accounts_supported: false\napi_keys_supported: false\ntoken_type: OAuth 2.0 user access token (Bearer)\nauthorization_server:\n  issuer: https://accounts.google.com\n  metadata: well-known/google-admob-oauth-authorization-server.json\n  openid_configuration: well-known/google-admob-openid-configuration.json\ncross_links:\n  scopes: scopes/google-admob-scopes.yml\n  conventions: conventions/google-admob-conventions.yml\n  errors:\
  \ errors/google-admob-problem-types.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/google-admob/refs/heads/main/authentication/google-admob-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Ad Mediation
- AdMob
- Advertising
- App Monetization
- Mobile Advertising
- Mobile Apps
- Reports
- Reporting
---
