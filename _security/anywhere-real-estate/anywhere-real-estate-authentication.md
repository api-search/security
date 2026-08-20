---
api_key_in:
- header
auth_types:
- oauth2
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Anywhere Real Estate Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: Anywhere Real Estate secures its APIs with oauth2 and apiKey across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: Anywhere Real Estate
provider_slug: anywhere-real-estate
scheme_count: 2
schemes:
- description: Anywhere-issued API key, provisioned per application per environment from the developer portal Dashboard > My Apps. Verbatim from the OAuth guide - "Every call to the APIs requires an API Key. This key must be passed in the request header as apiKey."
  in: header
  issued_by: developer portal (My Apps), after Anywhere approval
  name: AnywhereApiKey
  parameter_name: apiKey
  rotation:
    docs: https://developers.anywhere.re/blog/api-key-rotation-user-guide
    expires: true
    notes: API keys expire. The portal exposes a Renew Key action 45 days before expiry and sends an automated email; renewal is only possible up to the day of expiry. Anywhere ships a dual-mode API Key Rotation engine with downloadable toolkits for AWS (Lambda extension layer), Azure, local/on-prem and a manual path.
    renewal_window_days: 45
    supported: true
  sources:
  - https://developers.anywhere.re/docs/realogy-oauth
  type: apiKey
- authorization_endpoint_production: https://realogy.okta.com/oauth2/aus7i8b1taFyPOEGc1t7/v1/authorize
  client_credentials_delivery: The Postman walkthrough instructs developers to send the client credentials as HTTP Basic Auth (Okta Client ID as username, Client Secret as password) with a x-www-form-urlencoded body carrying grant_type=client_credentials and scope; the OAuth guide's own Postman steps say to send client credentials in the body. Both client_secret_basic and client_secret_post are advertised by the authorization server.
  code_challenge_methods_supported:
  - S256
  flow: clientCredentials
  grant_type: client_credentials
  introspection_endpoint_production: https://realogy.okta.com/oauth2/aus7i8b1taFyPOEGc1t7/v1/introspect
  jwks_uri_production: https://realogy.okta.com/oauth2/aus7i8b1taFyPOEGc1t7/v1/keys
  name: AnywhereOAuth2
  request_header: 'Authorization: Bearer {access_token}'
  response_fields:
  - access_token
  - token_type
  - expires_in
  - scope
  revocation_endpoint_production: https://realogy.okta.com/oauth2/aus7i8b1taFyPOEGc1t7/v1/revoke
  sources:
  - https://developers.anywhere.re/docs/realogy-oauth
  - authentication/anywhere-real-estate-okta-prod-authorization-server.json
  token_endpoint_auth_methods_supported:
  - client_secret_basic
  - client_secret_post
  - client_secret_jwt
  - private_key_jwt
  - none
  token_endpoint_non_production: https://realogy.oktapreview.com/oauth2/ausdtpyw647fbrcPi0h7/v1/token
  token_endpoint_production: https://realogy.okta.com/oauth2/aus7i8b1taFyPOEGc1t7/v1/token
  token_type: bearer
  type: oauth2
slug: anywhere-real-estate-authentication
source_filename: anywhere-real-estate-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-26'\nmethod: searched\nsource: https://developers.anywhere.re/docs/realogy-oauth\ndocs: https://developers.anywhere.re/docs/realogy-oauth\nsupporting_sources:\n- https://developers.anywhere.re/blog/test-anywhere-apis-postman-collection\n- https://developers.anywhere.re/blog/generate-bearer-token-using-api-credentials\n- https://developers.anywhere.re/blog/api-key-rotation-user-guide\n- authentication/anywhere-real-estate-okta-prod-authorization-server.json\n- authentication/anywhere-real-estate-okta-prod-openid-configuration.json\n- authentication/anywhere-real-estate-okta-nonprod-authorization-server.json\nsummary:\n  types: [oauth2, apiKey]\n  api_key_in: [header]\n  api_key_name: apiKey\n  oauth2_flows: [clientCredentials]\n  dual_credential: true\n  note: >-\n    Every call to an Anywhere API requires BOTH credentials — an Anywhere-issued API\n    key in the apiKey header AND an Okta-issued OAuth 2.0 bearer token obtained with\n    the client_credentials\
  \ grant. Neither alone is sufficient. The two credentials do\n    different jobs, stated verbatim in the OAuth guide: \"API keys identify the calling\n    application and make the call to an API. Authentication tokens identify a user that\n    is using the application.\"\nidentity_provider:\n  vendor: Okta\n  production_org: https://realogy.okta.com\n  non_production_org: https://realogy.oktapreview.com\n  federation: >-\n    Developer Portal release 1.3.30 (February 5, 2026) added federated authentication\n    with Compass Okta for Compass internal users, following the January 9, 2026\n    combination of Anywhere Real Estate and Compass.\nschemes:\n- name: AnywhereApiKey\n  type: apiKey\n  in: header\n  parameter_name: apiKey\n  description: >-\n    Anywhere-issued API key, provisioned per application per environment from the\n    developer portal Dashboard > My Apps. Verbatim from the OAuth guide - \"Every call\n    to the APIs requires an API Key. This key must be passed in the request\
  \ header as\n    apiKey.\"\n  issued_by: developer portal (My Apps), after Anywhere approval\n  rotation:\n    supported: true\n    expires: true\n    renewal_window_days: 45\n    notes: >-\n      API keys expire. The portal exposes a Renew Key action 45 days before expiry and\n      sends an automated email; renewal is only possible up to the day of expiry.\n      Anywhere ships a dual-mode API Key Rotation engine with downloadable toolkits for\n      AWS (Lambda extension layer), Azure, local/on-prem and a manual path.\n    docs: https://developers.anywhere.re/blog/api-key-rotation-user-guide\n  sources: [https://developers.anywhere.re/docs/realogy-oauth]\n- name: AnywhereOAuth2\n  type: oauth2\n  flow: clientCredentials\n  grant_type: client_credentials\n  token_endpoint_production: https://realogy.okta.com/oauth2/aus7i8b1taFyPOEGc1t7/v1/token\n  token_endpoint_non_production: https://realogy.oktapreview.com/oauth2/ausdtpyw647fbrcPi0h7/v1/token\n  authorization_endpoint_production:\
  \ https://realogy.okta.com/oauth2/aus7i8b1taFyPOEGc1t7/v1/authorize\n  jwks_uri_production: https://realogy.okta.com/oauth2/aus7i8b1taFyPOEGc1t7/v1/keys\n  introspection_endpoint_production: https://realogy.okta.com/oauth2/aus7i8b1taFyPOEGc1t7/v1/introspect\n  revocation_endpoint_production: https://realogy.okta.com/oauth2/aus7i8b1taFyPOEGc1t7/v1/revoke\n  token_endpoint_auth_methods_supported:\n  - client_secret_basic\n  - client_secret_post\n  - client_secret_jwt\n  - private_key_jwt\n  - none\n  code_challenge_methods_supported: [S256]\n  client_credentials_delivery: >-\n    The Postman walkthrough instructs developers to send the client credentials as HTTP\n    Basic Auth (Okta Client ID as username, Client Secret as password) with a\n    x-www-form-urlencoded body carrying grant_type=client_credentials and scope; the\n    OAuth guide's own Postman steps say to send client credentials in the body. Both\n    client_secret_basic and client_secret_post are advertised by the authorization\n\
  \    server.\n  response_fields: [access_token, token_type, expires_in, scope]\n  token_type: bearer\n  request_header: 'Authorization: Bearer {access_token}'\n  sources:\n  - https://developers.anywhere.re/docs/realogy-oauth\n  - authentication/anywhere-real-estate-okta-prod-authorization-server.json\nscopes:\n  model: App ID URI\n  reference: scopes/anywhere-real-estate-scopes.yml\n  caution: >-\n    Anywhere scopes are App ID URIs, not URLs to call. The OAuth guide warns verbatim\n    \"The App ID URI is a unique identifier for the REST API. It is not where the REST\n    API is hosted.\" REST API URLs are communicated separately per environment after\n    approval.\n  assignment: >-\n    \"Scope: Will be communicated in the final approval\" — scopes are granted per\n    approved application, not self-selected.\noperational_rules:\n- rule: mandatory token caching\n  text: >-\n    Verbatim - \"All access tokens have an expiration and must be cached by the\n    application within 5 minutes\
  \ of expiration. Applications who fail to cache their\n    access tokens and request new access tokens for every REST API call they make will\n    have their access immediately suspended.\"\n  enforcement: immediate suspension\n- rule: client secret handling\n  text: >-\n    Verbatim - \"Always store the client secret key securely... This should never be\n    stored in a Mobile App or Native App.\" A replacement secret can be requested on\n    suspected compromise.\n- rule: separate credentials per application\n  text: >-\n    Verbatim - \"Each client application must have separate credentials set and the API\n    Key.\"\n- rule: separate credentials per environment\n  text: >-\n    Sandbox and production are independently approved and independently credentialed;\n    each approval takes up to 2 business days.\nobserved:\n- probe: https://api.anywhere.re/mls/v1\n  status: 401\n  body: '{\"statusCode\":401,\"message\":\"Failed to resolve API Key variable apiKey\"}'\n  note: >-\n    The\
  \ gateway rejects an anonymous call on the API-key check before it ever evaluates\n    the bearer token, confirming apiKey is enforced at the Apigee layer.\n  date: '2026-07-26'\ngaps:\n- No mutualTLS, no openIdConnect discovery advertised on the API gateway itself.\n- No public OpenAPI, so securitySchemes cannot be verified per operation; this profile\n  is built entirely from the anonymously published OAuth guide plus harvested Okta\n  discovery documents.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/anywhere-real-estate/refs/heads/main/authentication/anywhere-real-estate-authentication.yml
summary_line: oauth2/apiKey · 2 schemes
tags:
- Real-Estate
- United States
- Property Listings
- MLS
- RESO
- Brokerage
- Franchising
- PropTech
- Title
- Escrow
- Relocation
- Leads
- Transaction
---
