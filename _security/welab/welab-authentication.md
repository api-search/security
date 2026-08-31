---
api_key_in: []
auth_types:
- mutualTLS
description: ''
kind: authentication
layout: security
method: probed
name: Welab Authentication
name_suffix: Authentication
oauth_flows: []
overview: WeLab secures its APIs with mutualTLS across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: WeLab
provider_slug: welab
scheme_count: 1
schemes:
- description: Both the production gateway (api.welab.bank) and the sandbox gateway (api-sandbox.welab.bank) require a client certificate at the TLS layer. The sandbox gateway completes the TLS 1.3 handshake, sends a CertificateRequest, and then answers an anonymous HTTP/2 request with 400 "No required SSL certificate was sent" (nginx). No path, method or payload is reachable without a WeLab-issued client certificate.
  hosts:
  - api.welab.bank
  - api-sandbox.welab.bank
  name: clientCertificate
  sources:
  - probe:https://api-sandbox.welab.bank/
  type: mutualTLS
slug: welab-authentication
source_filename: welab-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-05'\nmethod: probed\nsource: https://api-sandbox.welab.bank/\ndocs: https://portal-sandbox.welab.bank/\nnote: >-\n  Derived from live transport-layer probes of WeLab Bank's Open API gateways, not from a published\n  specification — WeLab Bank publishes no anonymous OpenAPI, and its developer portal is registration-gated,\n  so the application-layer credential model (token endpoints, scopes, header names) could not be observed.\n  What IS observable and certain is that both gateways terminate TLS with a client-certificate request and\n  refuse any request that does not present one.\nsummary:\n  types:\n  - mutualTLS\n  api_key_in: []\n  oauth2_flows: []\n  registration: required\n  registration_note: >-\n    Access to the sandbox and to the API catalogue requires registration with WeLab Bank as a third-party\n    service provider (TSP), consistent with the Hong Kong Monetary Authority Open API Framework, under which\n    account-information APIs require a\
  \ bank-onboarded TSP.\nschemes:\n- name: clientCertificate\n  type: mutualTLS\n  description: >-\n    Both the production gateway (api.welab.bank) and the sandbox gateway (api-sandbox.welab.bank) require a\n    client certificate at the TLS layer. The sandbox gateway completes the TLS 1.3 handshake, sends a\n    CertificateRequest, and then answers an anonymous HTTP/2 request with 400 \"No required SSL certificate\n    was sent\" (nginx). No path, method or payload is reachable without a WeLab-issued client certificate.\n  sources:\n  - probe:https://api-sandbox.welab.bank/\n  hosts:\n  - api.welab.bank\n  - api-sandbox.welab.bank\nx-evidence:\n  checked: '2026-08-05'\n  probes:\n  - url: https://api-sandbox.welab.bank/\n    http_status: 400\n    server: nginx\n    body: '400 No required SSL certificate was sent'\n    tls: TLSv1.3\n    tls_certificate_request: true\n    cert_subject: CN=api-sandbox.welab.bank\n    cert_issuer: C=US; O=Amazon; CN=Amazon RSA 2048 M01\n  - url: https://api.welab.bank/\n\
  \    http_status: 0\n    note: TCP connect timeout after 8s from a US network; A record resolves to prod-opa-gw-public-nlb (AWS ap-east-1, Hong Kong)\n  - url: https://portal-sandbox.welab.bank/\n    http_status: 403\n    note: Cloudflare \"Attention Required\" block page; the same 403 is returned to a browser user-agent and to WebFetch\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/welab/refs/heads/main/authentication/welab-authentication.yml
summary_line: mutualTLS · 1 scheme
tags:
- Fintech
- digital-banking
- virtual-bank
- open-banking
- hong-kong
- indonesia
- consumer-lending
- Payments
- hkma-open-api
- Financial-Services
---
