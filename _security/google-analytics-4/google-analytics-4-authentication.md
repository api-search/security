---
api_key_in: []
api_specs:
- filename: google-analytics-4-data-v1beta-openapi.yml
  format: yaml
  label: Google Analytics Data API
  slug: google-analytics-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/google-analytics-4/refs/heads/main/openapi/google-analytics-4-data-v1beta-openapi.yml
- filename: google-analytics-4-admin-v1beta-openapi.yml
  format: yaml
  label: Google Analytics Admin API
  slug: google-analytics-admin-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/google-analytics-4/refs/heads/main/openapi/google-analytics-4-admin-v1beta-openapi.yml
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Google Analytics 4 Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Google Analytics 4 secures its APIs with http and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Google Analytics 4
provider_slug: google-analytics-4
scheme_count: 2
schemes:
- description: Google OAuth 2.0. Scopes are the short form of the full https://www.googleapis.com/auth/<scope> identifier.
  flows:
  - authorizationUrl: https://accounts.google.com/o/oauth2/v2/auth
    flow: authorizationCode
    scopes: 4
    tokenUrl: https://oauth2.googleapis.com/token
  name: OAuth2
  sources:
  - openapi/google-analytics-4-admin-v1alpha-openapi.yml
  - openapi/google-analytics-4-admin-v1beta-openapi.yml
  - openapi/google-analytics-4-data-v1alpha-openapi.yml
  - openapi/google-analytics-4-data-v1beta-openapi.yml
  type: oauth2
- description: Google OAuth 2.0 access token presented as a bearer token.
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/google-analytics-4-admin-v1alpha-openapi.yml
  - openapi/google-analytics-4-admin-v1beta-openapi.yml
  - openapi/google-analytics-4-data-v1alpha-openapi.yml
  - openapi/google-analytics-4-data-v1beta-openapi.yml
  type: http
slug: google-analytics-4-authentication
source_filename: google-analytics-4-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: searched\ndocs:\n  - https://developers.google.com/analytics/devguides/reporting/data/v1/basics#authentication\n  - https://developers.google.com/analytics/devguides/config/admin/v1/rest\n  - https://developers.google.com/analytics/devguides/collection/protocol/ga4\n  - https://cloud.google.com/docs/authentication/provide-credentials-adc\nsource: openapi/google-analytics-4-admin-v1alpha-openapi.yml, openapi/google-analytics-4-admin-v1beta-openapi.yml,\n  openapi/google-analytics-4-data-v1alpha-openapi.yml, openapi/google-analytics-4-data-v1beta-openapi.yml\nsummary:\n  types:\n  - http\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: OAuth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://accounts.google.com/o/oauth2/v2/auth\n    tokenUrl: https://oauth2.googleapis.com/token\n    scopes: 4\n  description: Google OAuth 2.0. Scopes are the short form of the full https://www.googleapis.com/auth/<scope>\n\
  \    identifier.\n  sources:\n  - openapi/google-analytics-4-admin-v1alpha-openapi.yml\n  - openapi/google-analytics-4-admin-v1beta-openapi.yml\n  - openapi/google-analytics-4-data-v1alpha-openapi.yml\n  - openapi/google-analytics-4-data-v1beta-openapi.yml\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  description: Google OAuth 2.0 access token presented as a bearer token.\n  sources:\n  - openapi/google-analytics-4-admin-v1alpha-openapi.yml\n  - openapi/google-analytics-4-admin-v1beta-openapi.yml\n  - openapi/google-analytics-4-data-v1alpha-openapi.yml\n  - openapi/google-analytics-4-data-v1beta-openapi.yml\ncredential_types:\n  - type: oauth2-user\n    description: Three-legged OAuth for acting as an end user with access to a property.\n    grant: authorization_code\n  - type: service-account\n    description: >-\n      The standard machine-to-machine path. A Google service account is granted a role on the\n      GA4 property, then authenticates with the jwt-bearer grant. This\
  \ is what Application\n      Default Credentials resolves to in a server or CI environment, and what Google's own\n      client libraries and the official MCP server use.\n    grant: urn:ietf:params:oauth:grant-type:jwt-bearer\n    docs: https://cloud.google.com/docs/authentication/provide-credentials-adc\n  - type: api-key\n    supported: false\n    description: >-\n      Google API keys do NOT work against the Data or Admin API. Both require an OAuth\n      identity; a key-only request returns 401 UNAUTHENTICATED.\nmeasurement_protocol:\n  host: https://www.google-analytics.com\n  path: /mp/collect\n  eu_host: https://region1.google-analytics.com\n  scheme: shared-secret in query string\n  parameters:\n    - name: api_secret\n      in: query\n      required: true\n      description: >-\n        Server-side secret minted per data stream via\n        properties_dataStreams_measurementProtocolSecrets_create on the Admin API. Not\n        retrievable in plaintext from the console afterwards.\n\
  \    - name: measurement_id\n      in: query\n      required_for: web data streams\n    - name: firebase_app_id\n      in: query\n      required_for: app data streams\n  oauth: false\n  note: >-\n    The Measurement Protocol is the one GA4 surface that does not use OAuth at all. It is not\n    represented in any Discovery document or OpenAPI file, so it does not appear in the\n    schemes list above - this block is the record of it.\nproject_prerequisite:\n  note: >-\n    Beyond credentials, the calling Google Cloud project must have the relevant API enabled or\n    every call returns 403 PERMISSION_DENIED regardless of property access.\n  apis:\n    - analyticsdata.googleapis.com\n    - analyticsadmin.googleapis.com\nauthorization_server:\n  issuer: https://accounts.google.com\n  authorization_endpoint: https://accounts.google.com/o/oauth2/v2/auth\n  token_endpoint: https://oauth2.googleapis.com/token\n  metadata: well-known/google-analytics-4-oauth-authorization-server.json\n  oidc_discovery:\
  \ well-known/google-analytics-4-openid-configuration.json\nscopes: scopes/google-analytics-4-scopes.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/google-analytics-4/refs/heads/main/authentication/google-analytics-4-authentication.yml
summary_line: http/oauth2 · 2 schemes
tags:
- Analytics
- Data Collection
- Marketing
- Measurement
- Mobile Analytics
- Reporting
- Web Analytics
- Attribution
- Audiences
- Event Tracking
---
