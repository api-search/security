---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: cora.com.br
  spf: true
hosts:
- cert_expires: Aug 24 09:11:55 2026 GMT
  host: www.cora.com.br
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  6 21:22:53 2026 GMT
  host: developers.cora.com.br
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 16 23:59:59 2026 GMT
  host: matls-clients.api.cora.com.br
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Cora Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Cora, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: Cora
provider_slug: cora
slug: cora-domain-security
source_filename: cora-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.cora.com.br\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 24 09:11:55 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: developers.cora.com.br\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  6 21:22:53 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: matls-clients.api.cora.com.br\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 16 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: cora.com.br\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cora/refs/heads/main/security/cora-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Banking
- Brazil
- Payments
- Pix
- Boleto
- Invoicing
- SMB
- Fintech
- Banking-as-a-Service
---
