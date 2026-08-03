---
api_key_in: []
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: May Mobility Fleet Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: May Mobility secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: May Mobility
provider_slug: may-mobility
scheme_count: 1
schemes:
- applies_to:
  - api: May Mobility Fleet Realtime API
    example: domain?token=access_token_here&...
    parameter: token
    placement: query
  - api: May Mobility Fleet Batch (REST) API
    format: Bearer {access_token}
    header: Authorization
    placement: header
  client_authentication: client_secret_basic
  client_authentication_detail: 'The reference sample sends `Authorization: Basic ${base64Token}` with a base64 token supplied by the Fleet API team, plus grant_type=client_credentials, client_id, client_secret and scope in an application/x-www-form-urlencoded body.'
  client_id: provisioned per account
  client_secret: provisioned per account
  flow: clientCredentials
  identity_provider: AWS Cognito
  name: cognitoClientCredentials
  response_field: access_token
  scopes_note: The `scope` value is documented as `provided-by-fleet-api-team` and differs between the Realtime and Batch APIs. See scopes/may-mobility-scopes.yml.
  scopes_published: false
  sources:
  - https://docs.maymobility.com/docs/fleet-api/connecting-to-fleet-api
  token_endpoint: null
  token_endpoint_note: 'Published as `url: ''provided-by-fleet-api-team''` in the reference code sample. The Cognito domain is issued per account and is not public.'
  type: oauth2
slug: may-mobility-fleet-authentication
source_filename: may-mobility-fleet-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-01'\nmethod: searched\nsource: https://docs.maymobility.com/docs/fleet-api/connecting-to-fleet-api\ndocs: https://docs.maymobility.com/docs/fleet-api/connecting-to-fleet-api\nnote: 'Derived by reading the provider''s published authentication page, not from an\n  OpenAPI document — May Mobility publishes no machine-readable contract. Every value\n  below is either quoted from the docs or explicitly recorded as not published.'\nsummary:\n  types: [oauth2]\n  oauth2_flows: [clientCredentials]\n  api_key_in: []\n  identity_provider: AWS Cognito\n  token_type: bearer\n  onboarding: manual\n  onboarding_note: 'Step 1 of the published flow is \"Contact Fleet API team at May\n    Mobility for provisioning an account.\" There is no self-service sign-up; there is\n    no public developer registration page.'\nschemes:\n- name: cognitoClientCredentials\n  type: oauth2\n  flow: clientCredentials\n  identity_provider: AWS Cognito\n  token_endpoint: null\n  token_endpoint_note:\
  \ 'Published as `url: ''provided-by-fleet-api-team''` in the\n    reference code sample. The Cognito domain is issued per account and is not\n    public.'\n  client_id: provisioned per account\n  client_secret: provisioned per account\n  client_authentication: client_secret_basic\n  client_authentication_detail: 'The reference sample sends `Authorization: Basic\n    ${base64Token}` with a base64 token supplied by the Fleet API team, plus\n    grant_type=client_credentials, client_id, client_secret and scope in an\n    application/x-www-form-urlencoded body.'\n  scopes_published: false\n  scopes_note: The `scope` value is documented as `provided-by-fleet-api-team` and\n    differs between the Realtime and Batch APIs. See scopes/may-mobility-scopes.yml.\n  response_field: access_token\n  applies_to:\n  - api: May Mobility Fleet Realtime API\n    placement: query\n    parameter: token\n    example: domain?token=access_token_here&...\n  - api: May Mobility Fleet Batch (REST) API\n    placement:\
  \ header\n    header: Authorization\n    format: 'Bearer {access_token}'\n  sources:\n  - https://docs.maymobility.com/docs/fleet-api/connecting-to-fleet-api\ntransport_security:\n  tls_required: true\n  evidence: 'Docs state \"Note: All connections are encrypted.\"'\n  mutual_tls: false\n  mutual_tls_note: May Mobility operates its own client-certificate intermediate CA\n    (May Mobility Intermediate CA ECC SLC) for internal applications, but mTLS is not\n    documented as a Fleet API requirement.\nx-findings:\n- id: token-in-query-string\n  severity: medium\n  detail: 'The Realtime (WebSocket) API accepts the bearer access token as a `token`\n    URL query parameter. Query-string credentials are recorded in server access logs,\n    browser history and referrer headers; RFC 6750 section 2.3 deprecates the URI\n    query parameter method. This is a common constraint of browser WebSocket clients\n    (which cannot set request headers), but it is worth noting as a real property of\n   \
  \ the contract rather than an omission.'\n- id: no-discovery-document\n  severity: low\n  detail: No /.well-known/openid-configuration or /.well-known/oauth-authorization-server\n    is served on any May Mobility host (both 404). Because the Cognito domain is\n    account-issued, no public discovery document exists for the authorization server\n    either.\n- id: no-token-lifetime-published\n  severity: low\n  detail: Token TTL, refresh behaviour and rate limits on the token endpoint are not\n    documented.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/may-mobility/refs/heads/main/authentication/may-mobility-fleet-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Company
- Autonomous Vehicles
- Transportation
- Mobility
- Robotaxi
- Fleet Management
- Telemetry
- Public Transit
- Automotive
- Streaming
---
