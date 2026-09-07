---
anonymous_access: false
api_key_in: []
auth_types: []
description: 'Authentication profile for the Clearstream API Platform (api.clearstream.com). Clearstream runs an OAuth 2.0 resource-owner password-credentials flow that it has hardened by requiring a mutual-TLS connection on every call — both to the token endpoint and to every resource endpoint. Credentials are not self-service: an API consumer is a technical user created inside the Xact Web Portal, and the X.509 client certificate and key are generated in the browser during that user''s creation. This profile is read from Clearstream''s own published developer guide and confirmed against live 403 responses; no OpenAPI securitySchemes block exists because Clearstream publishes its OpenAPI only inside the registration-gated Deutsche Börse Digital Business Platform catalogue.'
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Clearstream Authentication
name_suffix: Authentication
oauth_flows: []
overview: Clearstream declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Clearstream
provider_slug: clearstream
scheme_count: 2
schemes:
- client_authentication: none
  client_authentication_note: No OAuth 2.0 client_id / client_secret basic-auth header is required — Clearstream identifies the client from the mutual-TLS certificate plus the consumer password sent as form data. The guide states that a basic-auth header set to any placeholder value is accepted and ignored, for libraries that insist on sending one.
  flow: password
  grant_type: password
  id: oauth2-password-mtls
  label: OAuth 2.0 resource owner password credentials, over mutual TLS
  request_encoding: application/x-www-form-urlencoded
  request_parameters:
  - name: grant_type
    required: true
    value: password
  - name: scope
    note: Space separated. The literal scope `allow` is mandatory on every request and must be accompanied by at least one API-specific scope. Requesting an invalid scope returns a 400 whose body lists the scopes valid for that consumer.
    required: true
  - name: username
    note: The Xact API Consumer user id, e.g. the form a00012345_0012345.
    required: true
  - name: password
    note: The API consumer login password set during Xact user creation.
    required: true
  resource_usage: 'Authorization: Bearer ${ACCESS_TOKEN}'
  response:
    access_token: JWT bearer token
    expires_in: 3599
    refresh_token: issued
    scope: echoed back as the granted scope string
    token_type: Bearer
  token_endpoint: https://api.clearstream.com/authmanager/oauth2/access_token
  token_endpoint_test: https://api-t2s-test.clearstream.com/authmanager/oauth2/access_token
  type: oauth2
- client_ca_bundle: https://api.clearstream.com/client-cert-cacerts.pem
  client_certificate:
    binding: The client certificate Common Name (CN) must match the Xact user id carried in the OAuth 2.0 token subject. Observed verbatim in the live 403 body from https://api-t2s-test.clearstream.com/playground/v1/info on 2026-09-05.
    delivery: Two PEM files are generated and downloaded in the browser — a signing certificate/key pair and an SSL (TLS) certificate/key pair — named ocapi-{USERID}-{TYPE}.pem. The SSL file is the one used for the mutual-TLS connection.
    issued_by: Clearstream, during Xact Web Portal API Consumer creation
    validity: 2 years; expiry visible to Xact OU administrators in the credential details screen
  id: mutual-tls
  label: Mandatory mutual TLS (X.509 client certificate)
  scope_of_application: Every call to the Clearstream API Platform, including the OAuth token endpoint. Running without a proper CA chain or truststore ("insecure mode") is explicitly unsupported.
  server_trust:
    note: Clients must add the server CA chain to their truststore. Certificate pinning is explicitly unsupported, and Clearstream reserves the right to rotate API server certificates with no prior announcement.
    root_ca: DigiCert Global Root G2
  type: mutualTLS
slug: clearstream-authentication
source_filename: clearstream-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "specification: API Commons Authentication\nspecificationVersion: '0.1'\nprovider: Clearstream\nproviderId: clearstream\ngenerated: '2026-09-05'\nmodified: '2026-09-05'\nmethod: searched\nsource: >-\n  Clearstream API Developer Guide (Clearstream Banking S.A., August 2025) —\n  https://www.clearstream.com/caas/v1/media/2934048/data/3fa3fec668d8dd198e9bed4df879b26b/api-developer-guide.pdf\n  (HTTP 200, application/pdf), plus live unauthenticated probes of the Clearstream API\n  Platform pre-production host https://api-t2s-test.clearstream.com (HTTP 403 JSON envelopes\n  naming the required scopes) on 2026-09-05.\ndocs:\n  - https://www.clearstream.com/clearstream-en/res-library/connectivity/clearstream-api-services-2916788\n  - https://www.clearstream.com/caas/v1/media/2934048/data/3fa3fec668d8dd198e9bed4df879b26b/api-developer-guide.pdf\n  - https://docs.developer.deutsche-boerse.com/docs/consumer/mTLS-consumer\ndescription: >-\n  Authentication profile for the Clearstream API\
  \ Platform (api.clearstream.com). Clearstream\n  runs an OAuth 2.0 resource-owner password-credentials flow that it has hardened by requiring\n  a mutual-TLS connection on every call — both to the token endpoint and to every resource\n  endpoint. Credentials are not self-service: an API consumer is a technical user created\n  inside the Xact Web Portal, and the X.509 client certificate and key are generated in the\n  browser during that user's creation. This profile is read from Clearstream's own published\n  developer guide and confirmed against live 403 responses; no OpenAPI securitySchemes block\n  exists because Clearstream publishes its OpenAPI only inside the registration-gated Deutsche\n  Börse Digital Business Platform catalogue.\nschemes:\n  - id: oauth2-password-mtls\n    type: oauth2\n    flow: password\n    label: OAuth 2.0 resource owner password credentials, over mutual TLS\n    token_endpoint: https://api.clearstream.com/authmanager/oauth2/access_token\n    token_endpoint_test:\
  \ https://api-t2s-test.clearstream.com/authmanager/oauth2/access_token\n    grant_type: password\n    request_encoding: application/x-www-form-urlencoded\n    request_parameters:\n      - name: grant_type\n        value: password\n        required: true\n      - name: scope\n        required: true\n        note: >-\n          Space separated. The literal scope `allow` is mandatory on every request and must be\n          accompanied by at least one API-specific scope. Requesting an invalid scope returns a\n          400 whose body lists the scopes valid for that consumer.\n      - name: username\n        required: true\n        note: The Xact API Consumer user id, e.g. the form a00012345_0012345.\n      - name: password\n        required: true\n        note: The API consumer login password set during Xact user creation.\n    client_authentication: none\n    client_authentication_note: >-\n      No OAuth 2.0 client_id / client_secret basic-auth header is required — Clearstream\n      identifies\
  \ the client from the mutual-TLS certificate plus the consumer password sent as\n      form data. The guide states that a basic-auth header set to any placeholder value is\n      accepted and ignored, for libraries that insist on sending one.\n    response:\n      access_token: JWT bearer token\n      refresh_token: issued\n      token_type: Bearer\n      expires_in: 3599\n      scope: echoed back as the granted scope string\n    resource_usage: 'Authorization: Bearer ${ACCESS_TOKEN}'\n  - id: mutual-tls\n    type: mutualTLS\n    label: Mandatory mutual TLS (X.509 client certificate)\n    scope_of_application: >-\n      Every call to the Clearstream API Platform, including the OAuth token endpoint. Running\n      without a proper CA chain or truststore (\"insecure mode\") is explicitly unsupported.\n    client_certificate:\n      issued_by: Clearstream, during Xact Web Portal API Consumer creation\n      delivery: >-\n        Two PEM files are generated and downloaded in the browser —\
  \ a signing certificate/key\n        pair and an SSL (TLS) certificate/key pair — named ocapi-{USERID}-{TYPE}.pem. The SSL\n        file is the one used for the mutual-TLS connection.\n      validity: 2 years; expiry visible to Xact OU administrators in the credential details screen\n      binding: >-\n        The client certificate Common Name (CN) must match the Xact user id carried in the\n        OAuth 2.0 token subject. Observed verbatim in the live 403 body from\n        https://api-t2s-test.clearstream.com/playground/v1/info on 2026-09-05.\n    server_trust:\n      root_ca: DigiCert Global Root G2\n      note: >-\n        Clients must add the server CA chain to their truststore. Certificate pinning is\n        explicitly unsupported, and Clearstream reserves the right to rotate API server\n        certificates with no prior announcement.\n    client_ca_bundle: https://api.clearstream.com/client-cert-cacerts.pem\nauthorization:\n  model: >-\n    Two layers. Coarse-grained access\
  \ is the set of Clearstream API resources granted to the\n    Xact Organisation Unit and then to the individual API Consumer user; that grant is what\n    determines which OAuth scopes the token server will issue. Fine-grained access is a\n    per-API role model inside Xact — for example most User Management (SCIM2) calls additionally\n    require the SCIM Admin or SCIM Read-Only role on top of the Xact Web Portal User Management\n    API role.\n  onboarding_channel: >-\n    Existing Xact clients enable the service by sending an MT599 SWIFT message to\n    CEDELULLXXX (attn. PRGConnect) naming the API resources to link to their Organisation Unit.\n    Prospects contact the Clearstream Connectivity Helpdesk at connect@clearstream.com.\n  self_service: false\nerrors:\n  invalid_scope: 400 — response body enumerates the scopes valid for the consumer\n  wrong_parameter: 403 Forbidden from the authorisation server; cause visible only in the Xact OU audit log\n  wrong_host: >-\n    OAuth requests\
  \ sent to https://xact.clearstream.com are rejected; the token endpoint is on\n    https://api.clearstream.com (or the matching test host).\nobservations:\n  - fetched: '2026-09-05'\n    url: https://api-t2s-test.clearstream.com/playground/v1/info\n    http_status: 403\n    content_type: application/json; charset=utf-8\n    note: >-\n      Unauthenticated probe. Body names the mandatory `allow` scope, the API scope\n      `ocapi-playground-v1`, and the certificate-CN-to-token-subject binding rule.\n  - fetched: '2026-09-05'\n    url: https://api.clearstream.com/\n    http_status: 503\n    note: >-\n      The production API host was serving a \"Scheduled Maintenance\" page for every path at the\n      time of this pass, so production probes could not be completed; the pre-production host\n      api-t2s-test.clearstream.com was up and answered.\nmaintainers:\n  - FN: Kin Lane\n    email: kin@apievangelist.com\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/clearstream/refs/heads/main/authentication/clearstream-authentication.yml
summary_line: 2 schemes
tags:
- API Platform
- Capital Markets
- Collateral Management
- Custody
- Financial-Services
- ISO 15022
- ISO 20022
- Mutual TLS
- OAuth 2.0
- Post-Trade
- Post-Trade Infrastructure
- SCIM
- Securities
- Settlement
- Swift
---
