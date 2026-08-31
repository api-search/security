---
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
method: searched
name: Skykick Authentication
name_suffix: Authentication
oauth_flows: []
overview: SkyKick declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: SkyKick
provider_slug: skykick
scheme_count: 2
schemes:
- description: Azure API Management subscription key. Retrieved from the Cloud Services portal under Admin > User Profile > Developer API Access, where each subscription (e.g. the Partner subscription) exposes a Show link that reveals the key. Sent on both the token request and every resource request.
  evidence: https://skykick.developer.azure-api.net/getstarted
  id: apim_subscription_key
  in: header
  name: Ocp-Apim-Subscription-Key
  required: true
  type: apiKey
- description: 'OAuth 2.0 client credentials grant (RFC 6749 section 4.4). The token request is an application/x-www-form-urlencoded POST carrying grant_type=client_credentials and a scope, authenticated with HTTP Basic where the username is the ClientId and the password is the Secret. The resulting token is sent as "Authorization: Bearer <token>" on resource calls.'
  evidence: https://skykick.developer.azure-api.net/getstarted
  flow: clientCredentials
  id: oauth2_client_credentials
  request:
    body_params:
    - grant_type=client_credentials
    - scope=Partner
    content_type: application/x-www-form-urlencoded
    headers:
    - Ocp-Apim-Subscription-Key
    - 'Authorization: Basic base64(ClientId:Secret)'
    method: POST
    url: https://apis.cloudservices.connectwise.com/auth/token
  required: true
  scopes:
  - Partner
  - Distributor
  token_url: https://apis.cloudservices.connectwise.com/auth/token
  type: oauth2
slug: skykick-authentication
source_filename: skykick-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-28'\nmethod: searched\nsource: https://skykick.developer.azure-api.net/getstarted\ndocs: https://skykick.developer.azure-api.net/getstarted\napi: SkyKick Partner Integration API\nbase_url: https://apis.cloudservices.connectwise.com\nnote: >-\n  Derived from the provider's own public Get Started page rather than from an\n  OpenAPI document — SkyKick publishes no machine-readable contract. The page is\n  served by the ConnectWise Developer Portal on SkyKick's own Azure API Management\n  instance (skykick.developer.azure-api.net) and is the only substantive\n  anonymously readable API documentation the provider still serves after the\n  September 2024 ConnectWise acquisition retired skykick.com.\nsummary: >-\n  Two credentials are required on every call. An Azure API Management subscription\n  key identifies the calling application to the gateway, and an OAuth 2.0\n  client-credentials bearer token identifies the partner. Both are issued from the\n  Cloud Services\
  \ partner portal and require an administrator to enable \"Developer\n  Access\" on a user before any of it can be obtained.\nschemes:\n- id: apim_subscription_key\n  type: apiKey\n  in: header\n  name: Ocp-Apim-Subscription-Key\n  required: true\n  description: >-\n    Azure API Management subscription key. Retrieved from the Cloud Services\n    portal under Admin > User Profile > Developer API Access, where each\n    subscription (e.g. the Partner subscription) exposes a Show link that reveals\n    the key. Sent on both the token request and every resource request.\n  evidence: https://skykick.developer.azure-api.net/getstarted\n- id: oauth2_client_credentials\n  type: oauth2\n  flow: clientCredentials\n  token_url: https://apis.cloudservices.connectwise.com/auth/token\n  required: true\n  description: >-\n    OAuth 2.0 client credentials grant (RFC 6749 section 4.4). The token request\n    is an application/x-www-form-urlencoded POST carrying grant_type=client_credentials\n    and a\
  \ scope, authenticated with HTTP Basic where the username is the ClientId\n    and the password is the Secret. The resulting token is sent as\n    \"Authorization: Bearer <token>\" on resource calls.\n  request:\n    method: POST\n    url: https://apis.cloudservices.connectwise.com/auth/token\n    content_type: application/x-www-form-urlencoded\n    headers:\n    - Ocp-Apim-Subscription-Key\n    - 'Authorization: Basic base64(ClientId:Secret)'\n    body_params:\n    - grant_type=client_credentials\n    - scope=Partner\n  scopes:\n  - Partner\n  - Distributor\n  evidence: https://skykick.developer.azure-api.net/getstarted\ncredential_provisioning:\n  gated: true\n  steps:\n  - Sign in to the Cloud Services portal with an Administrator account.\n  - Admin > Manage Users > Add New User, with the Developer Access checkbox set.\n  - The new user signs in at developers.cloudservices.connectwise.com.\n  - Admin > User Profile > Developer API Access exposes the ClientId, Secret and subscription\
  \ keys.\n  portal: https://portal.cloudservices.connectwise.com/\n  developer_portal: https://developers.cloudservices.connectwise.com\n  note: >-\n    There is no self-service signup. Credentials can only be minted by an\n    administrator of an existing partner tenant, which is why this profile records\n    the API as gated rather than public.\nverification:\n  identity_endpoint: https://apis.cloudservices.connectwise.com/whoami\n  probed: '2026-08-28'\n  anonymous_status: 401\n  anonymous_body: '{\"Message\":\"Authorization has been denied for this request.\"}'\n  www_authenticate: Bearer\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/skykick/refs/heads/main/authentication/skykick-authentication.yml
summary_line: 2 schemes
tags:
- Company
- Backup
- Migration
- Microsoft 365
- Managed Service Providers
- SaaS Security
- Cloud Automation
- Data Protection
- Azure API Management
---
