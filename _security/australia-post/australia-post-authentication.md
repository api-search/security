---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: australia-post-endpoints-api-openapi.yml
  format: yaml
  label: Australia Post Endpoints API
  slug: australia-post-endpoints-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/australia-post/refs/heads/main/openapi/australia-post-endpoints-api-openapi.yml
auth_types:
- apiKey
- oauth2
description: ''
kind: authentication
layout: security
mechanism_count: 3
method: searched
name: Australia Post Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- clientCredentials
overview: Australia Post secures its APIs with apiKey and oauth2 across 3 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode and clientCredentials flow(s).
provider_name: Australia Post
provider_slug: australia-post
scheme_count: 3
schemes:
- in: header
  name: Bearer
  parameter: Authorization
  sources:
  - openapi/australia-post-agency-data-delivery-openapi.yml
  type: apiKey
- in: header
  name: ApiKeyAuth
  parameter: AUTH-KEY
  sources:
  - openapi/australia-post-endpoints-api-openapi.yml
  - openapi/australia-post-locations-v3-openapi.yml
  type: apiKey
- flows:
  - flow: clientCredentials
    scopes: 1
  - authorizationUrl: https://welcome.auspost.com.au/authorize
    flow: authorizationCode
    scopes: 1
    tokenUrl: https://welcome.auspost.com.au/oauth/token
  name: OIDCSecurity
  sources:
  - openapi/australia-post-international-export-tools-v3-openapi.yml
  type: oauth2
slug: australia-post-authentication
source_filename: australia-post-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-21'\nmethod: searched\nsource:\n- https://auspost.com.au/developers/help-support/about-our-apis/\n- https://auspost.com.au/developers/help-support/how-to-get-credentials/\n- https://developers.auspost.com.au/apis/shipping-and-tracking/info/api-resources/faq\n- openapi/australia-post-agency-data-delivery-openapi.yml, openapi/australia-post-endpoints-api-openapi.yml, openapi/australia-post-international-export-tools-v3-openapi.yml,\n  openapi/australia-post-locations-v3-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - oauth2\n  api_key_in:\n  - header\n  oauth2_flows:\n  - authorizationCode\n  - clientCredentials\nschemes:\n- name: Bearer\n  type: apiKey\n  in: header\n  parameter: Authorization\n  sources:\n  - openapi/australia-post-agency-data-delivery-openapi.yml\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: AUTH-KEY\n  sources:\n  - openapi/australia-post-endpoints-api-openapi.yml\n  - openapi/australia-post-locations-v3-openapi.yml\n\
  - name: OIDCSecurity\n  type: oauth2\n  flows:\n  - flow: clientCredentials\n    scopes: 1\n  - flow: authorizationCode\n    authorizationUrl: https://welcome.auspost.com.au/authorize\n    tokenUrl: https://welcome.auspost.com.au/oauth/token\n    scopes: 1\n  sources:\n  - openapi/australia-post-international-export-tools-v3-openapi.yml\ndocs: https://auspost.com.au/developers/help-support/about-our-apis/\ndocumented_credential_types:\n- type: API Key\n  how: Include the API Key in the request header when you call one of our API endpoints.\n  header: AUTH-KEY\n  note: Key can be restricted by HTTP referrer, IP address or iOS bundle (native apps).\n- type: Basic Auth\n  how: 'Authorization: Basic Base64(\"api_key_uuid\" + \":\" + \"api_key_password\")'\n  header: Authorization\n  note: Used by the Shipping and Tracking API together with an Account-Number header (per the S&T FAQ).\n  source: https://developers.auspost.com.au/apis/shipping-and-tracking/info/api-resources/faq\n- type: OAuth\
  \ 2.0 Client Credentials\n  note: For machine-to-machine apps; APIs secured by the new identity provider (Auth0) or the legacy identity provider\n    (AuthZ).\n- type: OAuth 2.0 Authorisation Code\n  note: Regular web apps; PKCE variant for single page and native apps.\napp_types:\n- Machine-to-machine (M2M)\n- Regular web applications\n- Single page web applications (SPA)\n- Native applications\nguidance: For best practice, only use API Key and Basic Auth with M2M apps.\ntransport: TLS 1.2 or above is required (Shipping and Tracking security considerations).\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/australia-post/refs/heads/main/authentication/australia-post-authentication.yml
summary_line: apiKey/oauth2 · 3 schemes
tags:
- Address Validation
- Click and Collect
- Delivery
- E-Commerce
- Labels
- Location
- Logistics
- Parcel Locker
- Postal
- Postage
- Shipping
- Tracking
- Australia
---
