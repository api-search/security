---
api_key_in:
- header
api_specs:
- filename: telus-insights-location-api.postman_collection.json
  format: json
  label: TELUS Insights Location API
  slug: telus-insights-location-api
  spec_type: Postman
  url: https://raw.githubusercontent.com/api-evangelist/telus/refs/heads/main/collections/telus-insights-location-api.postman_collection.json
auth_types:
- oauth2
- http
description: 'TELUS runs two completely different authentication models on its two publicly documented APIs. The Insights Location API uses OAuth 2.0 client credentials plus a mandatory customerId header; the TELUS Health CHR Enterprise API uses asymmetric, self-signed JWTs (RS512) where the consumer holds the private key and CHR holds the registered public key — there is no token endpoint and no client secret at all. Neither surface is self-serve: credentials on both sides are issued through a sales/onboarding process.'
kind: authentication
layout: security
method: searched
name: Telus Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: TELUS secures its APIs with oauth2 and http across 4 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: TELUS
provider_slug: telus
scheme_count: 4
schemes:
- access_token_use: 'Authorization: Bearer {access_token}'
  api: TELUS Insights Location API
  flow: clientCredentials
  name: InsightsOAuth2ClientCredentials
  request_parameters:
  - grant_type
  - client_id
  - client_secret
  - scope
  scopes_published: false
  sources:
  - collections/telus-insights-location-api.postman_collection.json
  - https://docs.insights.telus.com/
  token_lifetime_seconds: 299
  token_request_content_type: application/x-www-form-urlencoded
  token_reuse_guidance: '"When getting an OAuth Token from the Token URL, it is preferable that you reuse the token for specified amount of expiry seconds (present inside the token JSON and set to 299 seconds). That prevents the identity system from being overwhelmed."'
  token_url_note: The token endpoint is not published anonymously. The documentation instructs the consumer to read oauth_token_endpoint, oauth_grant_type and oauth_scope from the "My Account" page of the TELUS Insights Portal (https://insights.telus.com).
  token_url_published: false
  type: oauth2
- api: TELUS Insights Location API
  case_note: The published shell examples send the header lower-cased as `customerid`; the Postman collection sends `customerId` on count/shapefile/geofence/usage requests and `customerid` on the Job endpoints. HTTP header names are case-insensitive, so both are the same header.
  description: Tenant identifier that scopes every request to one customer. Documented as "the unique ID generated when 'Create Customer ID' is performed which creates the association of a customer with their unique API key." Required in addition to the bearer token on every operation.
  in: header
  name: InsightsCustomerIdHeader
  parameter_name: customerId
  required: true
  sources:
  - collections/telus-insights-location-api.postman_collection.json
  type: apiKey
- api: TELUS Health CHR Enterprise API
  bearerFormat: JWT
  client_secret: none
  header: 'Authorization: Bearer {json_web_token}'
  key_material: 2048-bit RSA key pair. The consumer generates it, keeps the private key, and registers the public key in PEM format in the "JWT Public Key" field of an API Consumer under Settings > Enterprise API in the CHR account.
  name: CHRSelfSignedJWT
  notes:
  - There is no authorization server and no token exchange — the consumer mints its own token.
  - Every API action is audit-logged; requests and responses are retained for 90 days.
  - Access is a paid feature enabled per CHR account, gated by a Privacy & Security questionnaire.
  required_claims:
  - claim: iss
    requirement: Must match the Issuer value configured on the API Consumer record in CHR.
  - claim: exp
    requirement: Must expire within the next 15 minutes (900 seconds).
  scheme: bearer
  signing_algorithm: RS512
  sources:
  - https://help.inputhealth.com/en/articles/6483215-chr-enterprise-api
  - https://help.inputhealth.com/en/articles/6483223-making-requests-to-the-api
  - https://help.inputhealth.com/en/articles/6483229-creating-api-consumers
  token_endpoint: none
  type: http
- api: TELUS Health CHR Enterprise API — Event Notification Service
  direction: inbound-to-consumer
  mechanism: The CHR signs each outbound event notification with a shared secret supplied by the consumer when creating the subscription; the resulting signature travels in a request header. The header name is not published in the help centre and was not verified.
  name: CHREventNotificationSignature
  sources:
  - https://help.inputhealth.com/en/articles/7988802-chr-enterprise-api-event-notifications
  type: webhookSignature
slug: telus-authentication
source_filename: telus-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-25'\nmethod: searched\nsource: >-\n  https://docs.insights.telus.com/ (TELUS Insights Location API, Postman Documenter) and\n  https://help.inputhealth.com/en/collections/3317215-chr-enterprise-api (TELUS Health CHR\n  Enterprise API). Cross-checked against the harvested Postman collection\n  (collections/telus-insights-location-api.postman_collection.json, auth type oauth2) and the\n  harvested GraphQL introspection document (graphql/telus-chr-enterprise-api-introspection.json).\ndescription: >-\n  TELUS runs two completely different authentication models on its two publicly documented APIs.\n  The Insights Location API uses OAuth 2.0 client credentials plus a mandatory customerId header;\n  the TELUS Health CHR Enterprise API uses asymmetric, self-signed JWTs (RS512) where the consumer\n  holds the private key and CHR holds the registered public key — there is no token endpoint and no\n  client secret at all. Neither surface is self-serve: credentials\
  \ on both sides are issued through\n  a sales/onboarding process.\nsummary:\n  types: [oauth2, http]\n  api_key_in: [header]\n  oauth2_flows: [clientCredentials]\n  jwt_bearer_self_signed: true\n  self_serve_credentials: false\nschemes:\n- name: InsightsOAuth2ClientCredentials\n  api: TELUS Insights Location API\n  type: oauth2\n  flow: clientCredentials\n  token_url_published: false\n  token_url_note: >-\n    The token endpoint is not published anonymously. The documentation instructs the consumer to\n    read oauth_token_endpoint, oauth_grant_type and oauth_scope from the \"My Account\" page of the\n    TELUS Insights Portal (https://insights.telus.com).\n  request_parameters: [grant_type, client_id, client_secret, scope]\n  token_request_content_type: application/x-www-form-urlencoded\n  access_token_use: 'Authorization: Bearer {access_token}'\n  token_lifetime_seconds: 299\n  token_reuse_guidance: >-\n    \"When getting an OAuth Token from the Token URL, it is preferable that you reuse\
  \ the token for\n    specified amount of expiry seconds (present inside the token JSON and set to 299 seconds). That\n    prevents the identity system from being overwhelmed.\"\n  scopes_published: false\n  sources: [collections/telus-insights-location-api.postman_collection.json, https://docs.insights.telus.com/]\n- name: InsightsCustomerIdHeader\n  api: TELUS Insights Location API\n  type: apiKey\n  in: header\n  parameter_name: customerId\n  case_note: >-\n    The published shell examples send the header lower-cased as `customerid`; the Postman collection\n    sends `customerId` on count/shapefile/geofence/usage requests and `customerid` on the Job\n    endpoints. HTTP header names are case-insensitive, so both are the same header.\n  description: >-\n    Tenant identifier that scopes every request to one customer. Documented as \"the unique ID\n    generated when 'Create Customer ID' is performed which creates the association of a customer with\n    their unique API key.\" Required\
  \ in addition to the bearer token on every operation.\n  required: true\n  sources: [collections/telus-insights-location-api.postman_collection.json]\n- name: CHRSelfSignedJWT\n  api: TELUS Health CHR Enterprise API\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  header: 'Authorization: Bearer {json_web_token}'\n  signing_algorithm: RS512\n  key_material: >-\n    2048-bit RSA key pair. The consumer generates it, keeps the private key, and registers the\n    public key in PEM format in the \"JWT Public Key\" field of an API Consumer under\n    Settings > Enterprise API in the CHR account.\n  required_claims:\n  - claim: iss\n    requirement: Must match the Issuer value configured on the API Consumer record in CHR.\n  - claim: exp\n    requirement: Must expire within the next 15 minutes (900 seconds).\n  token_endpoint: none\n  client_secret: none\n  notes:\n  - There is no authorization server and no token exchange — the consumer mints its own token.\n  - Every API action is audit-logged;\
  \ requests and responses are retained for 90 days.\n  - Access is a paid feature enabled per CHR account, gated by a Privacy & Security questionnaire.\n  sources:\n  - https://help.inputhealth.com/en/articles/6483215-chr-enterprise-api\n  - https://help.inputhealth.com/en/articles/6483223-making-requests-to-the-api\n  - https://help.inputhealth.com/en/articles/6483229-creating-api-consumers\n- name: CHREventNotificationSignature\n  api: TELUS Health CHR Enterprise API — Event Notification Service\n  type: webhookSignature\n  direction: inbound-to-consumer\n  mechanism: >-\n    The CHR signs each outbound event notification with a shared secret supplied by the consumer\n    when creating the subscription; the resulting signature travels in a request header. The header\n    name is not published in the help centre and was not verified.\n  sources: [https://help.inputhealth.com/en/articles/7988802-chr-enterprise-api-event-notifications]\nportal_authentication:\n- name: TELUS Client Identity\
  \ (PingFederate)\n  where: api.telus.com API Marketplace and insights.telus.com portal sign-in\n  type: oauth2\n  flow: authorizationCode\n  authorization_endpoint: https://auth-gateway.telus.com/as/authorization.oauth2\n  scopes_observed: [ciiLogin, identityinfofulldetail, serviceassociation]\n  note: Human browser sign-in for the portals, not an API grant. Discovery documents return 403 (Cloudflare).\nnot_found:\n  openid_connect_discovery: No /.well-known/openid-configuration is reachable on any TELUS host.\n  mtls: No mutual-TLS requirement is documented on either API.\n  ciba: >-\n    CIBA — the backchannel flow CAMARA specifies for network APIs — appears nowhere on a TELUS\n    property; TELUS publishes no first-party CAMARA endpoint.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/telus/refs/heads/main/authentication/telus-authentication.yml
summary_line: oauth2/http · 4 schemes
tags:
- Telecommunications
- Canada
- Mobile Network Operator
- Broadband
- Network APIs
- CAMARA
- Open Gateway
- SIM Swap
- Identity Verification
- Location Intelligence
- IoT
- 5G
- Healthcare
- Electronic Medical Records
- GraphQL
- Webhook
- Geospatial
---
