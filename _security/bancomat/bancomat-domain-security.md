---
api_specs:
- filename: bancomat-flowpay-api-v1-openapi.yml
  format: yaml
  label: FlowPay API (v1)
  slug: flowpay-api-v1
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bancomat/refs/heads/main/openapi/bancomat-flowpay-api-v1-openapi.yml
- filename: bancomat-flowpay-api-v2-openapi.yml
  format: yaml
  label: FlowPay API (v2)
  slug: flowpay-api-v2
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bancomat/refs/heads/main/openapi/bancomat-flowpay-api-v2-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: flowpay.it
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: bancomat.it
  spf: true
hosts:
- cert_expires: Oct 27 07:23:57 2026 GMT
  host: flowpay.it
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 16 22:22:09 2026 GMT
  host: bancomat.it
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 27 07:23:57 2026 GMT
  host: docs.flowpay.it
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 3
kind: domain-security
layout: security
method: probed
name: Bancomat Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Bancomat, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Bancomat
provider_slug: bancomat
slug: bancomat-domain-security
source_filename: bancomat-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: flowpay.it\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 27 07:23:57 2026 GMT\n  hsts: false\n- host: bancomat.it\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 16 22:22:09 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.flowpay.it\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 27 07:23:57 2026 GMT\n  hsts: false\ndomains:\n- domain: flowpay.it\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: bancomat.it\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bancomat/refs/heads/main/security/bancomat-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- ATM
- Banking
- Financial-Services
- Italy
- Mobile Payments
- Payments
- Debit Cards
- Open Banking
- PSD2
- Account Information
- Payment Initiation
- Invoicing
- pagoPA
---
