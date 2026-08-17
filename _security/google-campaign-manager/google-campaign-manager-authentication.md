---
api_key_in: []
api_specs:
- filename: google-campaign-manager-ads-api-openapi.yml
  format: yaml
  label: Google Campaign Manager Ads API
  slug: google-campaign-manager-ads-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/google-campaign-manager/refs/heads/main/openapi/google-campaign-manager-ads-api-openapi.yml
- filename: google-campaign-manager-campaigns-api-openapi.yml
  format: yaml
  label: Google Campaign Manager Campaigns API
  slug: google-campaign-manager-campaigns-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/google-campaign-manager/refs/heads/main/openapi/google-campaign-manager-campaigns-api-openapi.yml
- filename: google-campaign-manager-placements-api-openapi.yml
  format: yaml
  label: Google Campaign Manager Placements API
  slug: google-campaign-manager-placements-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/google-campaign-manager/refs/heads/main/openapi/google-campaign-manager-placements-api-openapi.yml
- filename: google-campaign-manager-reports-api-openapi.yml
  format: yaml
  label: Google Campaign Manager Reports API
  slug: google-campaign-manager-reports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/google-campaign-manager/refs/heads/main/openapi/google-campaign-manager-reports-api-openapi.yml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Google Campaign Manager Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- jwt-bearer
overview: Google Campaign Manager secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode and jwt-bearer flow(s).
provider_name: Google Campaign Manager
provider_slug: google-campaign-manager
scheme_count: 1
schemes:
- alternative_parameters:
  - access_token
  - oauth_token
  description: OAuth 2.0 is the only way in. Google's global `key` query parameter is accepted by the endpoint but does not authorise access to Campaign Manager user data.
  flows:
  - authorizationUrl: https://accounts.google.com/o/oauth2/v2/auth
    flow: authorizationCode
    refresh: Request access_type=offline and prompt=consent to receive a refresh token; without it a long-running integration cannot re-authenticate.
    revocationUrl: https://oauth2.googleapis.com/revoke
    scopes: 3
    tokenUrl: https://oauth2.googleapis.com/token
  - description: Service account with domain-wide delegation, impersonating a Google Workspace user who holds a Campaign Manager 360 user profile. This is the supported unattended path — a bare service account with no delegation cannot see Campaign Manager data.
    docs: https://developers.google.com/doubleclick-advertisers/service_accounts
    flow: jwt-bearer
  name: OAuth2
  sources:
  - https://developers.google.com/doubleclick-advertisers/authorizing
  - openapi/google-campaign-manager-ads-api-openapi.yml
  - openapi/google-campaign-manager-campaigns-api-openapi.yml
  - openapi/google-campaign-manager-placements-api-openapi.yml
  - openapi/google-campaign-manager-reports-api-openapi.yml
  token_presentation: 'Authorization: Bearer <access_token>'
  type: oauth2
slug: google-campaign-manager-authentication
source_filename: google-campaign-manager-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: searched\nsource: >-\n  https://developers.google.com/doubleclick-advertisers/authorizing,\n  https://developers.google.com/doubleclick-advertisers/service_accounts,\n  https://dfareporting.googleapis.com/$discovery/rest?version=v5,\n  well-known/google-campaign-manager-oauth-authorization-server.json\ndocs: https://developers.google.com/doubleclick-advertisers/authorizing\nprovider: Google Campaign Manager\nproviderId: google-campaign-manager\nsummary:\n  types:\n    - oauth2\n  oauth2_flows:\n    - authorizationCode\n    - jwt-bearer\n  api_key: false\n  mtls: false\nschemes:\n  - name: OAuth2\n    type: oauth2\n    flows:\n      - flow: authorizationCode\n        authorizationUrl: https://accounts.google.com/o/oauth2/v2/auth\n        tokenUrl: https://oauth2.googleapis.com/token\n        revocationUrl: https://oauth2.googleapis.com/revoke\n        scopes: 3\n        refresh: >-\n          Request access_type=offline and prompt=consent to\
  \ receive a refresh\n          token; without it a long-running integration cannot re-authenticate.\n      - flow: jwt-bearer\n        description: >-\n          Service account with domain-wide delegation, impersonating a Google\n          Workspace user who holds a Campaign Manager 360 user profile. This is\n          the supported unattended path — a bare service account with no\n          delegation cannot see Campaign Manager data.\n        docs: https://developers.google.com/doubleclick-advertisers/service_accounts\n    token_presentation: 'Authorization: Bearer <access_token>'\n    alternative_parameters:\n      - access_token\n      - oauth_token\n    description: >-\n      OAuth 2.0 is the only way in. Google's global `key` query parameter is\n      accepted by the endpoint but does not authorise access to Campaign Manager\n      user data.\n    sources:\n      - https://developers.google.com/doubleclick-advertisers/authorizing\n      - openapi/google-campaign-manager-ads-api-openapi.yml\n\
  \      - openapi/google-campaign-manager-campaigns-api-openapi.yml\n      - openapi/google-campaign-manager-placements-api-openapi.yml\n      - openapi/google-campaign-manager-reports-api-openapi.yml\nauthorization_server:\n  issuer: https://accounts.google.com\n  metadata:\n    - url: https://accounts.google.com/.well-known/oauth-authorization-server\n      status: 200\n      file: well-known/google-campaign-manager-oauth-authorization-server.json\n    - url: https://accounts.google.com/.well-known/openid-configuration\n      status: 200\n      file: well-known/google-campaign-manager-openid-configuration.json\n  protected_resource_metadata:\n    url: https://dfareporting.googleapis.com/.well-known/oauth-protected-resource\n    status: 404\n    note: >-\n      RFC 9728 metadata is not served, so a client cannot discover the\n      authorization server from the API host.\nauthorization_model:\n  tenant_selector: profileId\n  note: >-\n    A valid token is not sufficient. Every data path\
  \ is\n    /userprofiles/{profileId}/..., and the profile determines which account and\n    which objects are visible. Resolve it with userProfiles.list, then treat it\n    as part of the credential.\n  role_model: >-\n    Fine-grained permissions live in Campaign Manager 360 user roles\n    (userRoles, userRolePermissions, accountPermissions), not in OAuth scopes.\n    The three scopes are coarse — there is no read-only scope.\nobserved:\n  - url: https://dfareporting.googleapis.com/dfareporting/v5/userprofiles\n    status: 401\n    body_status: UNAUTHENTICATED\n    reason: required\n    checked: '2026-08-13'\n    note: >-\n      The 401 response carries no WWW-Authenticate challenge pointing at the\n      authorization server; the error body names a documentation URL instead.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/google-campaign-manager/refs/heads/main/authentication/google-campaign-manager-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Advertising
- Analytics
- Campaign Management
- Digital Marketing
- Reporting
- Ad Serving
- Ad Trafficking
- Attribution
- Conversion Tracking
- Marketing
- Media Buying
- Google Marketing Platform
---
