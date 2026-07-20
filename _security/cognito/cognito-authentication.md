---
api_key_in:
- header
auth_types:
- httpSignature
description: 'Cognito authenticates every API request with HTTP request signatures (the Cavage "Signing HTTP Messages" draft), not a bearer token or HTTP Basic. Each request carries a Date header, a Digest header (base64 SHA-256 of the body), and an Authorization: Signature header whose signature is an HMAC-SHA256 over the "(request-target) date digest" signing string, keyed with the API secret. The API key (keyId) identifies the organization; the API secret is used only server-side to compute the signature and is never transmitted.'
kind: authentication
layout: security
method: searched
name: Cognito Authentication
name_suffix: Authentication
oauth_flows: []
overview: Cognito secures its APIs with httpSignature across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Cognito
provider_slug: cognito
scheme_count: 1
schemes:
- algorithm: hmac-sha256
  clock_skew: Date must be within 15 minutes of server time (per webhook verification docs)
  headers:
    Authorization: Signature keyId="<api-key>",algorithm="hmac-sha256",headers="(request-target) date digest",signature="<base64 hmac-sha256 signature>"
    Date: W3C/RFC 1123 timestamp, e.g. "Thu, 25 Aug 2016 22:37:14 GMT"
    Digest: SHA-256=<base64(sha256(body))>
  key_id: API key (keyId)
  name: HTTPSignature
  scheme: signature
  secret: API secret (HMAC key, never transmitted)
  signed_headers:
  - (request-target)
  - date
  - digest
  sources:
  - docs
  type: http
slug: cognito-authentication
source_filename: cognito-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: https://cognitohq.com/docs/guides/authenticating\ndocs: https://cognitohq.com/docs/guides/authenticating\ndescription: >-\n  Cognito authenticates every API request with HTTP request signatures (the\n  Cavage \"Signing HTTP Messages\" draft), not a bearer token or HTTP Basic. Each\n  request carries a Date header, a Digest header (base64 SHA-256 of the body),\n  and an Authorization: Signature header whose signature is an HMAC-SHA256 over\n  the \"(request-target) date digest\" signing string, keyed with the API secret.\n  The API key (keyId) identifies the organization; the API secret is used only\n  server-side to compute the signature and is never transmitted.\nsummary:\n  types: [httpSignature]\n  api_key_in: [header]\n  oauth2_flows: []\nschemes:\n- name: HTTPSignature\n  type: http\n  scheme: signature\n  algorithm: hmac-sha256\n  key_id: API key (keyId)\n  secret: API secret (HMAC key, never transmitted)\n  signed_headers:\n\
  \  - (request-target)\n  - date\n  - digest\n  headers:\n    Date: W3C/RFC 1123 timestamp, e.g. \"Thu, 25 Aug 2016 22:37:14 GMT\"\n    Digest: \"SHA-256=<base64(sha256(body))>\"\n    Authorization: >-\n      Signature keyId=\"<api-key>\",algorithm=\"hmac-sha256\",headers=\"(request-target)\n      date digest\",signature=\"<base64 hmac-sha256 signature>\"\n  clock_skew: Date must be within 15 minutes of server time (per webhook verification docs)\n  sources: [docs]\nnotes: >-\n  Community and beta SDKs implement the signing so integrators do not compute the\n  HMAC by hand. No OpenAPI spec was located to derive from; profile captured from\n  the published authentication guide.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cognito/refs/heads/main/authentication/cognito-authentication.yml
summary_line: httpSignature · 1 scheme
tags:
- Company
- Identity
- Identity Verification
- KYC
- AML
- Compliance
- Fraud Prevention
- Onboarding
- Watchlist Screening
- Know Your Customer
---
