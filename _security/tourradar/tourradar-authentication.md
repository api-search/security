---
api_key_in: []
auth_types:
- oauth2
- openIdConnect
description: ''
kind: authentication
layout: security
method: searched
name: Tourradar Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: TourRadar secures its APIs with oauth2 and openIdConnect across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: TourRadar
provider_slug: tourradar
scheme_count: 2
schemes:
- description: OAuth 2.0 for the TourRadar B2B Distribution API, fronted by oauth.api.b2b.tourradar.com and backed by an AWS Cognito user pool.
  endpoints:
    authorization: https://auth.tourradar.com/oauth2/authorize
    cognito_hosted_domain: https://b2b-tourradar-production.auth.us-east-1.amazoncognito.com
    login_spa: https://login.tourradar.com
    oauth: https://oauth.api.b2b.tourradar.com
    revocation: https://auth.tourradar.com/oauth2/revoke
  name: TourRadarB2BOAuth
  scopes_count: 24
  scopes_ref: scopes/tourradar-scopes.yml
  type: oauth2
- description: OpenID Connect discovery for the B2B partner identity pool (openid, email, profile scopes).
  discovery_file: well-known/tourradar-openid-configuration.json
  discovery_status: 200
  name: TourRadarB2BOIDC
  openIdConnectUrl: https://cognito-idp.us-east-1.amazonaws.com/us-east-1_AzhYLFMIv/.well-known/openid-configuration
  type: openIdConnect
slug: tourradar-authentication
source_filename: tourradar-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://dashboard.api.b2b.tourradar.com/config.js\ndocs: https://www.tourradar.com/distribution-api\nnotes: >-\n  TourRadar's Distribution API (B2B partner platform for OTAs, airlines and GDSs)\n  authenticates partners with OAuth 2.0 / OpenID Connect issued by an AWS Cognito\n  user pool (us-east-1_AzhYLFMIv). The partner dashboard's public config.js exposes\n  the OAuth endpoint, the Cognito hosted domain, the client id used by the dashboard\n  SPA, and the full resource-server scope list. The API itself (api.b2b.tourradar.com)\n  rejects unauthenticated requests (HTTP 403). Detailed developer documentation sits\n  behind the partner dashboard login (dashboard.api.b2b.tourradar.com/docs).\nsummary:\n  types: [oauth2, openIdConnect]\n  oauth2_flows: [authorizationCode]\n  issuer: https://cognito-idp.us-east-1.amazonaws.com/us-east-1_AzhYLFMIv\nschemes:\n  - name: TourRadarB2BOAuth\n    type: oauth2\n    description: OAuth\
  \ 2.0 for the TourRadar B2B Distribution API, fronted by oauth.api.b2b.tourradar.com and backed by an AWS Cognito user pool.\n    endpoints:\n      oauth: https://oauth.api.b2b.tourradar.com\n      authorization: https://auth.tourradar.com/oauth2/authorize\n      revocation: https://auth.tourradar.com/oauth2/revoke\n      cognito_hosted_domain: https://b2b-tourradar-production.auth.us-east-1.amazoncognito.com\n      login_spa: https://login.tourradar.com\n    scopes_count: 24\n    scopes_ref: scopes/tourradar-scopes.yml\n  - name: TourRadarB2BOIDC\n    type: openIdConnect\n    description: OpenID Connect discovery for the B2B partner identity pool (openid, email, profile scopes).\n    openIdConnectUrl: https://cognito-idp.us-east-1.amazonaws.com/us-east-1_AzhYLFMIv/.well-known/openid-configuration\n    discovery_status: 200\n    discovery_file: well-known/tourradar-openid-configuration.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tourradar/refs/heads/main/authentication/tourradar-authentication.yml
summary_line: oauth2/openIdConnect · 2 schemes
tags:
- Travel
- Tours
- Booking
- Marketplace
- Adventure Travel
- Distribution
- Affiliates
---
