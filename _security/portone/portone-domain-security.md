---
api_specs:
- filename: portone-openapi.yml
  format: yaml
  label: PortOne Payments API (V2)
  slug: portone-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/portone/refs/heads/main/openapi/portone-openapi.yml
- filename: portone-openapi.yml
  format: yaml
  label: PortOne Billing Keys API (V2)
  slug: portone-billing-keys-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/portone/refs/heads/main/openapi/portone-openapi.yml
- filename: portone-openapi.yml
  format: yaml
  label: PortOne Payment Schedule API (V2)
  slug: portone-payment-schedules-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/portone/refs/heads/main/openapi/portone-openapi.yml
- filename: portone-openapi.yml
  format: yaml
  label: PortOne Identity Verification API (V2)
  slug: portone-identity-verification-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/portone/refs/heads/main/openapi/portone-openapi.yml
- filename: portone-openapi.yml
  format: yaml
  label: PortOne Cash Receipts API (V2)
  slug: portone-cash-receipts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/portone/refs/heads/main/openapi/portone-openapi.yml
- filename: portone-openapi.yml
  format: yaml
  label: PortOne B2B Tax Invoice API (V2)
  slug: portone-b2b-tax-invoice-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/portone/refs/heads/main/openapi/portone-openapi.yml
- filename: portone-openapi.yml
  format: yaml
  label: PortOne Platform Partner Settlement API (V2)
  slug: portone-platform-partner-settlement-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/portone/refs/heads/main/openapi/portone-openapi.yml
- filename: portone-openapi.yml
  format: yaml
  label: PortOne Payment Sessions & Checkout API (V2)
  slug: portone-payment-sessions-checkout-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/portone/refs/heads/main/openapi/portone-openapi.yml
- filename: portone-openapi.yml
  format: yaml
  label: PortOne Payment Reconciliation API (V2)
  slug: portone-payment-reconciliation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/portone/refs/heads/main/openapi/portone-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dmarc_rua: mailto:infra+dmarc@portone.io
  dnssec: false
  domain: portone.io
  spf: true
  spf_record: v=spf1 include:_spf.google.com include:mail.stibee.com include:_spf.salesforce.com include:_spf.getresponse.com include:243569856.spf05.hubspotemail.net ~all
hosts:
- cert_expires: Oct  2 15:06:23 2026 GMT
  cert_issuer: (probed)
  host: portone.io
  http_status: 308
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 29 23:59:59 2026 GMT
  cert_issuer: C=US, O=Amazon, CN=Amazon RSA 2048 M04
  host: api.portone.io
  http_status: 404
  https: true
  notes: V2 API host; served behind AWS. Root path returns 404 (no unauthenticated index).
  tls_version: TLSv1.3
- cert_expires: Sep 24 18:31:39 2026 GMT
  host: developers.portone.io
  http_status: 200
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 18 23:59:59 2027 GMT
  host: api.iamport.kr
  http_status: 301
  https: true
  notes: Legacy V1 (Iamport) API host, still live.
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Portone Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for PortOne, probed live across 4 host(s) and 1 registrable domain(s). 4 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: PortOne
provider_slug: portone
slug: portone-domain-security
source_filename: portone-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: portone.io\n  https: true\n  tls_version: TLSv1.3\n  http_status: 308\n  cert_expires: Oct  2 15:06:23 2026 GMT\n  cert_issuer: (probed)\n- host: api.portone.io\n  https: true\n  tls_version: TLSv1.3\n  http_status: 404\n  cert_expires: Nov 29 23:59:59 2026 GMT\n  cert_issuer: 'C=US, O=Amazon, CN=Amazon RSA 2048 M04'\n  notes: V2 API host; served behind AWS. Root path returns 404 (no unauthenticated index).\n- host: developers.portone.io\n  https: true\n  tls_version: TLSv1.3\n  http_status: 200\n  cert_expires: Sep 24 18:31:39 2026 GMT\n- host: api.iamport.kr\n  https: true\n  tls_version: TLSv1.3\n  http_status: 301\n  cert_expires: Jan 18 23:59:59 2027 GMT\n  notes: Legacy V1 (Iamport) API host, still live.\ndomains:\n- domain: portone.io\n  dnssec: false\n  caa: []\n  spf: true\n  spf_record: 'v=spf1 include:_spf.google.com include:mail.stibee.com include:_spf.salesforce.com\
  \ include:_spf.getresponse.com include:243569856.spf05.hubspotemail.net ~all'\n  dmarc: true\n  dmarc_policy: none\n  dmarc_rua: 'mailto:infra+dmarc@portone.io'\nnotes: >-\n  All apis.yml and OpenAPI hosts serve over HTTPS with TLS 1.3. The V2 API host\n  api.portone.io presents an Amazon-issued certificate (AWS-fronted). A\n  .well-known/security.txt was not found on portone.io (HTTP 404) at probe time.\n  DMARC is published with policy p=none (monitoring). No CAA records were returned\n  for portone.io. The legacy api.iamport.kr host remains live for V1 integrations.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/portone/refs/heads/main/security/portone-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Payments
- Payment Orchestration
- Fintech
- Korea
- Billing
- Identity Verification
---
