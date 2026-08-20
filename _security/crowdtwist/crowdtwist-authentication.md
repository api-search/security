---
api_key_in: []
api_specs:
- filename: crowdtwist-starter-kit.postman_collection.json
  format: json
  label: Oracle CrowdTwist Loyalty and Engagement API
  slug: crowdtwist-loyalty
  spec_type: Postman
  url: https://raw.githubusercontent.com/api-evangelist/crowdtwist/refs/heads/main/postman/crowdtwist-starter-kit.postman_collection.json
auth_types: []
description: ''
kind: authentication
layout: security
method: searched
name: Crowdtwist Authentication
name_suffix: Authentication
oauth_flows: []
overview: CrowdTwist declares 5 security scheme(s) across its OpenAPI definitions.
provider_name: CrowdTwist
provider_slug: crowdtwist
scheme_count: 5
schemes:
- applies_to: all api[client_id].crowdtwist.com endpoints
  description: The client API key, issued by the CrowdTwist account team and visible in the CrowdTwist Control Center. Sent on nearly every documented v2/v2.1/v2.2 endpoint as `?api_key=`.
  evidence: https://docs.oracle.com/en/cloud/saas/marketing/crowdtwist-develop/Developers/UserCreate.html
  id: api_key_query
  in: query
  name: api_key
  required: true
  type: apiKey
- description: The same client API key presented as a header instead of a query parameter. Oracle's docs note explicitly that there is a single space between `CTApiKey` and the key value. This is the documented form on the POS/commerce endpoints (purchase, fulfillment, return).
  evidence: https://docs.oracle.com/en/cloud/saas/marketing/crowdtwist-develop/Developers/Purchase.html
  id: api_key_header
  in: header
  name: X-CT-Authorization
  required: false
  type: apiKey
  value_format: CTApiKey <API Key>
- algorithm: HMAC-SHA-256
  constraints:
  - Supported on api[client_id].crowdtwist.com; NOT supported on pos[client_id].crowdtwist.com.
  - Not supported on the legacy Auth Sign-In and Sign-Out endpoints.
  - When HMAC is enabled, an API key in the request URL is no longer required.
  description: 'Optional request signing, enabled per client. Headers are `X-CT-Authorization: CTApiV2Auth <public key>:<signature>` and `X-CT-Timestamp: <unix ms>`, where signature = Base64(HMAC-SHA-256(PrivateKey, StringToSign)) and StringToSign = HTTP-Verb + "\n" + Content-MD5 + "\n" + Content-Type + "\n" + Timestamp + "\n" + RequestURI.'
  evidence: https://docs.oracle.com/en/cloud/saas/marketing/crowdtwist-develop/Developers/HMACAuthentication.html
  id: hmac_v2
  replay_protection:
    header: X-CT-Timestamp
    mechanism: timestamp window
    window: 15 minutes
  required: false
  scheme: signature
  type: http
- description: End-user / mobile authentication. A user is first created via the User Create API, then authenticated against an alternate HMAC-enabled endpoint that returns a user session token and key which must be included in all subsequent calls. Requests to these endpoints must be HMAC signed with the HMAC *user* private key from the client's API configuration.
  evidence: https://docs.oracle.com/en/cloud/saas/marketing/crowdtwist-develop/Developers/MobileAPIAuthentication.html
  id: mobile_user_token
  in: header
  name: user session token
  required: false
  token_lifetime: 6 months
  type: apiKey
- description: Legacy signature parameter on the program-hosted single sign-on endpoints `POST https://<program_url>/http/v2/auth-sign-in` and `GET https://<program_url>/http/v2/auth-sign-out`. These run on the client's own program domain rather than the CrowdTwist API host and are explicitly excluded from HMAC support.
  evidence: https://docs.oracle.com/en/cloud/saas/marketing/crowdtwist-develop/Developers/UserAuthenticationSignIn.html
  id: api_sig_legacy
  in: query
  name: api_sig
  required: true
  type: apiKey
slug: crowdtwist-authentication
source_filename: crowdtwist-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: searched\nsource: https://docs.oracle.com/en/cloud/saas/marketing/crowdtwist-develop/Developers/HMACAuthentication.html\ndocs:\n- https://docs.oracle.com/en/cloud/saas/marketing/crowdtwist-develop/Developers/HMACAuthentication.html\n- https://docs.oracle.com/en/cloud/saas/marketing/crowdtwist-develop/Developers/MobileAPIAuthentication.html\n- https://docs.oracle.com/en/cloud/saas/marketing/crowdtwist-develop/Developers/EndpointURLEnvironments.html\napi: Oracle CrowdTwist Loyalty and Engagement REST API\nsummary: >-\n  CrowdTwist authenticates server-to-server traffic with a per-client API key, which may be\n  sent either as an `api_key` query-string parameter or in an `X-CT-Authorization` header.\n  Clients who enable it can upgrade to HMAC-SHA-256 request signing over the same key pair.\n  End-user (mobile) traffic uses a separate HMAC-signed authentication endpoint that returns\n  a six-month user session token. There is no OAuth 2.0, no OpenID\
  \ Connect and no published\n  scope model on this API.\nschemes:\n- id: api_key_query\n  type: apiKey\n  in: query\n  name: api_key\n  required: true\n  description: >-\n    The client API key, issued by the CrowdTwist account team and visible in the CrowdTwist\n    Control Center. Sent on nearly every documented v2/v2.1/v2.2 endpoint as `?api_key=`.\n  applies_to: all api[client_id].crowdtwist.com endpoints\n  evidence: https://docs.oracle.com/en/cloud/saas/marketing/crowdtwist-develop/Developers/UserCreate.html\n- id: api_key_header\n  type: apiKey\n  in: header\n  name: X-CT-Authorization\n  value_format: 'CTApiKey <API Key>'\n  required: false\n  description: >-\n    The same client API key presented as a header instead of a query parameter. Oracle's docs\n    note explicitly that there is a single space between `CTApiKey` and the key value. This is\n    the documented form on the POS/commerce endpoints (purchase, fulfillment, return).\n  evidence: https://docs.oracle.com/en/cloud/saas/marketing/crowdtwist-develop/Developers/Purchase.html\n\
  - id: hmac_v2\n  type: http\n  scheme: signature\n  algorithm: HMAC-SHA-256\n  required: false\n  description: >-\n    Optional request signing, enabled per client. Headers are `X-CT-Authorization:\n    CTApiV2Auth <public key>:<signature>` and `X-CT-Timestamp: <unix ms>`, where signature =\n    Base64(HMAC-SHA-256(PrivateKey, StringToSign)) and StringToSign = HTTP-Verb + \"\\n\" +\n    Content-MD5 + \"\\n\" + Content-Type + \"\\n\" + Timestamp + \"\\n\" + RequestURI.\n  replay_protection:\n    mechanism: timestamp window\n    window: 15 minutes\n    header: X-CT-Timestamp\n  constraints:\n  - Supported on api[client_id].crowdtwist.com; NOT supported on pos[client_id].crowdtwist.com.\n  - Not supported on the legacy Auth Sign-In and Sign-Out endpoints.\n  - When HMAC is enabled, an API key in the request URL is no longer required.\n  evidence: https://docs.oracle.com/en/cloud/saas/marketing/crowdtwist-develop/Developers/HMACAuthentication.html\n- id: mobile_user_token\n  type: apiKey\n\
  \  in: header\n  name: user session token\n  required: false\n  description: >-\n    End-user / mobile authentication. A user is first created via the User Create API, then\n    authenticated against an alternate HMAC-enabled endpoint that returns a user session token\n    and key which must be included in all subsequent calls. Requests to these endpoints must be\n    HMAC signed with the HMAC *user* private key from the client's API configuration.\n  token_lifetime: 6 months\n  evidence: https://docs.oracle.com/en/cloud/saas/marketing/crowdtwist-develop/Developers/MobileAPIAuthentication.html\n- id: api_sig_legacy\n  type: apiKey\n  in: query\n  name: api_sig\n  required: true\n  description: >-\n    Legacy signature parameter on the program-hosted single sign-on endpoints\n    `POST https://<program_url>/http/v2/auth-sign-in` and\n    `GET https://<program_url>/http/v2/auth-sign-out`. These run on the client's own program\n    domain rather than the CrowdTwist API host and are explicitly\
  \ excluded from HMAC support.\n  evidence: https://docs.oracle.com/en/cloud/saas/marketing/crowdtwist-develop/Developers/UserAuthenticationSignIn.html\noauth2: false\nopenid_connect: false\nmtls: false\nscopes_published: false\nscopes_note: >-\n  CrowdTwist has no OAuth surface, so there is no scope model to capture; access is scoped by\n  the client program the API key belongs to. scopes/ is deliberately absent for this provider.\ninbound_vs_outbound:\n  note: >-\n    The Data Push (webhook) direction reverses the relationship — CrowdTwist is the CALLER and\n    authenticates to the client's endpoint with HTTP Basic or a client-supplied `x-api-key`\n    header. See asyncapi/crowdtwist-data-push-webhooks.yml.\nkey_management:\n  issuance: CrowdTwist account team / CrowdTwist Control Center Dashboard\n  self_service: false\n  rotation_documented: false\n  separate_sandbox_keys: true\n  sandbox_note: Sandbox environments are separate hosts (sb-, sb2-) with their own client configuration.\n\
  transport:\n  tls_minimum: TLSv1.2\n  tls_note: >-\n    Oracle publishes the exact supported cipher suite list on the API Best Practices page and\n    warns that clients on runtimes without TLS 1.2 (e.g. Java 6) cannot connect.\n  evidence: https://docs.oracle.com/en/cloud/saas/marketing/crowdtwist-develop/Developers/CrowdTwistAPIBestPractices.html\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/crowdtwist/refs/heads/main/authentication/crowdtwist-authentication.yml
summary_line: 5 schemes
tags:
- Company
- Loyalty
- Customer Engagement
- Marketing
- Gamification
- Rewards
- Oracle
- CX Marketing
- Loyalty Programs
- Points
- Retail
- Commerce
- Segmentation
- Webhook
---
