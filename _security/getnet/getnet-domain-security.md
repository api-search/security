---
api_specs:
- filename: webook-sap
  format: yaml
  label: Getnet SAP Immediate Delivery APIs
  slug: getnet-sap-immediate-delivery
  spec_type: AsyncAPI
  url: https://docs.globalgetnet.com/en/products/sap-immediate-delivery/webook-sap
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: globalgetnet.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: getnet.com.br
  spf: true
hosts:
- cert_expires: Dec  8 23:59:59 2026 GMT
  host: docs.globalgetnet.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec  9 23:59:59 2026 GMT
  host: api.getnet.com.br
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  5 23:59:59 2026 GMT
  host: developers.getnet.com.br
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Getnet Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Getnet, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Getnet
provider_slug: getnet
slug: getnet-domain-security
source_filename: getnet-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: docs.globalgetnet.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  8 23:59:59 2026 GMT\n  hsts: false\n- host: api.getnet.com.br\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  9 23:59:59 2026 GMT\n  hsts: null\n- host: developers.getnet.com.br\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  5 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: globalgetnet.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: getnet.com.br\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/getnet/refs/heads/main/security/getnet-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Payments
- Acquirer
- Brazil
- LATAM
- Santander
- E-Commerce
- In-Store Payments
- POS
- Pix
- Boleto
- Cards
- 3DS
- Tokenization
- Marketplace
- Split Payments
- Payment Link
- Web Checkout
- Onboarding
- Chargeback
- Webhooks
- OAuth 2.0
- Agentic Commerce
- MCP
---
