---
api_key_in: []
api_specs:
- filename: vibes-platform-api-openapi.json
  format: json
  label: Vibes Platform API
  slug: vibes-platform-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vibes-platform/refs/heads/main/openapi/vibes-platform-api-openapi.json
- filename: vibes-platform-rcs-business-messaging-openapi.json
  format: json
  label: Vibes RCS Business Messaging API
  slug: vibes-rcs-business-messaging-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vibes-platform/refs/heads/main/openapi/vibes-platform-rcs-business-messaging-openapi.json
- filename: vibes-platform-acquisition-campaigns-api-openapi.yml
  format: yaml
  label: Vibes Platform Acquisition Campaigns API
  slug: vibes-platform-acquisition-campaigns-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vibes-platform/refs/heads/main/openapi/vibes-platform-acquisition-campaigns-api-openapi.yml
- filename: vibes-platform-broadcasts-api-openapi.yml
  format: yaml
  label: Vibes Platform Broadcasts API
  slug: vibes-platform-broadcasts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vibes-platform/refs/heads/main/openapi/vibes-platform-broadcasts-api-openapi.yml
- filename: vibes-platform-callbacks-api-openapi.yml
  format: yaml
  label: Vibes Platform Callbacks API
  slug: vibes-platform-callbacks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vibes-platform/refs/heads/main/openapi/vibes-platform-callbacks-api-openapi.yml
- filename: vibes-platform-carrier-lookup-api-openapi.yml
  format: yaml
  label: Vibes Platform Carrier Lookup API
  slug: vibes-platform-carrier-lookup-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vibes-platform/refs/heads/main/openapi/vibes-platform-carrier-lookup-api-openapi.yml
- filename: vibes-platform-events-api-openapi.yml
  format: yaml
  label: Vibes Platform Events API
  slug: vibes-platform-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vibes-platform/refs/heads/main/openapi/vibes-platform-events-api-openapi.yml
- filename: vibes-platform-inbound-messages-api-openapi.yml
  format: yaml
  label: Vibes Platform Inbound Messages API
  slug: vibes-platform-inbound-messages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vibes-platform/refs/heads/main/openapi/vibes-platform-inbound-messages-api-openapi.yml
- filename: vibes-platform-messages-api-openapi.yml
  format: yaml
  label: Vibes Platform Messages API
  slug: vibes-platform-messages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vibes-platform/refs/heads/main/openapi/vibes-platform-messages-api-openapi.yml
- filename: vibes-platform-persons-api-openapi.yml
  format: yaml
  label: Vibes Platform Persons API
  slug: vibes-platform-persons-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vibes-platform/refs/heads/main/openapi/vibes-platform-persons-api-openapi.yml
- filename: vibes-platform-subscription-lists-api-openapi.yml
  format: yaml
  label: Vibes Platform Subscription Lists API
  slug: vibes-platform-subscription-lists-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vibes-platform/refs/heads/main/openapi/vibes-platform-subscription-lists-api-openapi.yml
- filename: vibes-platform-wallet-passes-api-openapi.yml
  format: yaml
  label: Vibes Platform Wallet Passes API
  slug: vibes-platform-wallet-passes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vibes-platform/refs/heads/main/openapi/vibes-platform-wallet-passes-api-openapi.yml
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Vibes Platform Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: Vibes Platform secures its APIs with http and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: Vibes Platform
provider_slug: vibes-platform
scheme_count: 2
schemes:
- description: HTTP Basic Authentication. Combine the username and password into a "username:password" string, encode it using Base64, and add the Authorization HTTP header set to "Basic " plus the encoded string.
  name: basicAuth
  scheme: basic
  sources:
  - openapi/vibes-platform-acquisition-campaigns-api-openapi.yml
  - openapi/vibes-platform-api-openapi.json
  - openapi/vibes-platform-broadcasts-api-openapi.yml
  - openapi/vibes-platform-callbacks-api-openapi.yml
  - openapi/vibes-platform-carrier-lookup-api-openapi.yml
  - openapi/vibes-platform-events-api-openapi.yml
  - openapi/vibes-platform-inbound-messages-api-openapi.yml
  - openapi/vibes-platform-messages-api-openapi.yml
  - openapi/vibes-platform-persons-api-openapi.yml
  - openapi/vibes-platform-rbm-authentication-openapi.json
  - openapi/vibes-platform-subscription-lists-api-openapi.yml
  - openapi/vibes-platform-wallet-passes-api-openapi.yml
  type: http
- flows:
  - flow: clientCredentials
    scopes: 1
    tokenUrl: https://vibes-rbm-prd.auth.us-west-2.amazoncognito.com/oauth2/token
  name: OAuth2Auth
  sources:
  - openapi/vibes-platform-rcs-business-messaging-openapi.json
  type: oauth2
slug: vibes-platform-authentication
source_filename: vibes-platform-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: searched\ndocs: https://developer-platform.vibes.com/reference/technical-details\ndocs_additional:\n  - https://developer-platform.vibes.com/docs/client-certificate-authentication-for-vibes-apis\n  - https://developer-aggregation.vibes.com/reference/authentication-1\nsource: openapi/vibes-platform-acquisition-campaigns-api-openapi.yml, openapi/vibes-platform-api-openapi.json,\n  openapi/vibes-platform-broadcasts-api-openapi.yml, openapi/vibes-platform-callbacks-api-openapi.yml,\n  openapi/vibes-platform-carrier-lookup-api-openapi.yml, openapi/vibes-platform-events-api-openapi.yml,\n  openapi/vibes-platform-inbound-messages-api-openapi.yml, openapi/vibes-platform-messages-api-openapi.yml,\n  openapi/vibes-platform-persons-api-openapi.yml, openapi/vibes-platform-rbm-authentication-openapi.json,\n  openapi/vibes-platform-rcs-business-messaging-openapi.json, openapi/vibes-platform-subscription-lists-api-openapi.yml\n  ...\nsummary:\n  types:\n \
  \ - http\n  - oauth2\n  oauth2_flows:\n  - clientCredentials\nschemes:\n- name: basicAuth\n  type: http\n  scheme: basic\n  description: HTTP Basic Authentication. Combine the username and password into a \"username:password\"\n    string, encode it using Base64, and add the Authorization HTTP header set to \"Basic \" plus\n    the encoded string.\n  sources:\n  - openapi/vibes-platform-acquisition-campaigns-api-openapi.yml\n  - openapi/vibes-platform-api-openapi.json\n  - openapi/vibes-platform-broadcasts-api-openapi.yml\n  - openapi/vibes-platform-callbacks-api-openapi.yml\n  - openapi/vibes-platform-carrier-lookup-api-openapi.yml\n  - openapi/vibes-platform-events-api-openapi.yml\n  - openapi/vibes-platform-inbound-messages-api-openapi.yml\n  - openapi/vibes-platform-messages-api-openapi.yml\n  - openapi/vibes-platform-persons-api-openapi.yml\n  - openapi/vibes-platform-rbm-authentication-openapi.json\n  - openapi/vibes-platform-subscription-lists-api-openapi.yml\n  - openapi/vibes-platform-wallet-passes-api-openapi.yml\n\
  - name: OAuth2Auth\n  type: oauth2\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://vibes-rbm-prd.auth.us-west-2.amazoncognito.com/oauth2/token\n    scopes: 1\n  sources:\n  - openapi/vibes-platform-rcs-business-messaging-openapi.json\ndocs_findings:\n  - scheme: basicAuth\n    published: true\n    detail: >-\n      Vibes' Technical Details page documents Basic auth construction step by step and warns that\n      usernames must DIFFER between the EU and US instances — credentials are not portable across\n      regions, which the OpenAPI does not say.\n    source: https://developer-platform.vibes.com/reference/technical-details\n  - scheme: clientCertificate\n    type: mutualTLS\n    published: true\n    in_spec: false\n    detail: >-\n      Vibes documents client certificate authentication as an optional additional layer on top of\n      Basic for API calls. It appears in NO securityScheme in any published spec, so a\n      spec-only reader would never learn it exists.\n \
  \   source: https://developer-platform.vibes.com/docs/client-certificate-authentication-for-vibes-apis\n  - scheme: OAuth2Auth\n    published: true\n    detail: >-\n      OAuth 2.0 client credentials, documented for the RCS Business Messaging API only. Token is\n      issued by a Vibes-operated AWS Cognito user pool and presented as\n      `Authorization: Bearer [access_token]`.\n    source: https://developer-aggregation.vibes.com/reference/authentication-1\nrequired_headers_note: >-\n  Authentication alone is not sufficient — X-API-Version must also be sent (see\n  conventions/vibes-platform-conventions.yml). Omitting it silently selects version 1, which cannot\n  handle E.164 phone numbers.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/vibes-platform/refs/heads/main/authentication/vibes-platform-authentication.yml
summary_line: http/oauth2 · 2 schemes
tags:
- Mobile Marketing
- Mobile Messaging
- Push Notifications
- SMS
- MMS
- Broadcast Messaging
- Acquisition Campaigns
- Subscription Management
- Wallet Passes
- RCS
---
