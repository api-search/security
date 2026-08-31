---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: facturama.mx
  spf: true
hosts:
- cert_expires: Sep 26 18:12:44 2026 GMT
  host: facturama.mx
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan  1 23:59:59 2027 GMT
  host: apisandbox.facturama.mx
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan  1 23:59:59 2027 GMT
  host: api.facturama.mx
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Facturama Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Facturama, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Facturama
provider_slug: facturama
slug: facturama-domain-security
source_filename: facturama-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: facturama.mx\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 26 18:12:44 2026 GMT\n  hsts: false\n- host: apisandbox.facturama.mx\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  1 23:59:59 2027 GMT\n  hsts: false\n- host: api.facturama.mx\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  1 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: facturama.mx\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/facturama/refs/heads/main/security/facturama-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Electronic Invoicing
- CFDI
- e-Invoicing
- Mexico
- Tax Compliance
- SAT
- Billing
- Payroll
- Finance
- REST API
---
