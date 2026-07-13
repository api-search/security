---
api_key_in: []
api_specs:
- filename: ownerrez-openapi.yml
  format: yaml
  label: OwnerRez Bookings API
  slug: ownerrez-bookings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ownerrez/refs/heads/main/openapi/ownerrez-openapi.yml
- filename: ownerrez-openapi.yml
  format: yaml
  label: OwnerRez Properties API
  slug: ownerrez-properties-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ownerrez/refs/heads/main/openapi/ownerrez-openapi.yml
- filename: ownerrez-openapi.yml
  format: yaml
  label: OwnerRez Listings API
  slug: ownerrez-listings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ownerrez/refs/heads/main/openapi/ownerrez-openapi.yml
- filename: ownerrez-openapi.yml
  format: yaml
  label: OwnerRez Guests API
  slug: ownerrez-guests-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ownerrez/refs/heads/main/openapi/ownerrez-openapi.yml
- filename: ownerrez-openapi.yml
  format: yaml
  label: OwnerRez Inquiries API
  slug: ownerrez-inquiries-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ownerrez/refs/heads/main/openapi/ownerrez-openapi.yml
- filename: ownerrez-openapi.yml
  format: yaml
  label: OwnerRez Quotes API
  slug: ownerrez-quotes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ownerrez/refs/heads/main/openapi/ownerrez-openapi.yml
- filename: ownerrez-openapi.yml
  format: yaml
  label: OwnerRez Reviews API
  slug: ownerrez-reviews-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ownerrez/refs/heads/main/openapi/ownerrez-openapi.yml
- filename: ownerrez-openapi.yml
  format: yaml
  label: OwnerRez Messages API
  slug: ownerrez-messages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ownerrez/refs/heads/main/openapi/ownerrez-openapi.yml
- filename: ownerrez-openapi.yml
  format: yaml
  label: OwnerRez Custom Fields and Tags API
  slug: ownerrez-custom-fields-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ownerrez/refs/heads/main/openapi/ownerrez-openapi.yml
- filename: ownerrez-openapi.yml
  format: yaml
  label: OwnerRez Payments and Financials API
  slug: ownerrez-financials-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ownerrez/refs/heads/main/openapi/ownerrez-openapi.yml
- filename: ownerrez-openapi.yml
  format: yaml
  label: OwnerRez Webhook Subscriptions API
  slug: ownerrez-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ownerrez/refs/heads/main/openapi/ownerrez-openapi.yml
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Ownerrez Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: OwnerRez secures its APIs with http and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: OwnerRez
provider_slug: ownerrez
scheme_count: 2
schemes:
- description: HTTP Basic authentication. Supply your OwnerRez API key / Personal Access Token as the username; the password is left blank.
  name: basicAuth
  scheme: basic
  sources:
  - openapi/ownerrez-openapi.yml
  type: http
- description: OAuth 2.0 Authorization Code Grant (RFC 6749 Section 4.1). Register an OAuth app in the OwnerRez Developer/API settings, send the user to the authorization URL, then exchange the returned code for an access token.
  flows:
  - authorizationUrl: https://app.ownerrez.com/oauth/authorize
    flow: authorizationCode
    scopes: 0
    tokenUrl: https://api.ownerrez.com/oauth/access_token
  name: oauth2
  sources:
  - openapi/ownerrez-openapi.yml
  type: oauth2
slug: ownerrez-authentication
source_filename: ownerrez-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/ownerrez-openapi.yml\nsummary:\n  types:\n  - http\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: basicAuth\n  type: http\n  scheme: basic\n  description: HTTP Basic authentication. Supply your OwnerRez API key / Personal Access Token\n    as the username; the password is left blank.\n  sources:\n  - openapi/ownerrez-openapi.yml\n- name: oauth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://app.ownerrez.com/oauth/authorize\n    tokenUrl: https://api.ownerrez.com/oauth/access_token\n    scopes: 0\n  description: OAuth 2.0 Authorization Code Grant (RFC 6749 Section 4.1). Register an OAuth\n    app in the OwnerRez Developer/API settings, send the user to the authorization URL, then\n    exchange the returned code for an access token.\n  sources:\n  - openapi/ownerrez-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ownerrez/refs/heads/main/authentication/ownerrez-authentication.yml
summary_line: http/oauth2 · 2 schemes
tags:
- Vacation Rental
- Short-Term Rental
- Property Management
- Hospitality
- Bookings
- Channel Manager
---
