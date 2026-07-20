---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: flowpay.io
  spf: true
hosts:
- cert_expires: Aug 20 23:41:36 2026 GMT
  host: flowpay.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  7 13:45:44 2026 GMT
  host: developers.flowpay.io
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 26 19:34:00 2026 GMT
  host: api.flowpay.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Flowpayio Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for flowpay.io, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: flowpay.io
provider_slug: flowpayio
slug: flowpayio-domain-security
source_filename: flowpayio-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: flowpay.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 20 23:41:36 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developers.flowpay.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  7 13:45:44 2026 GMT\n  hsts: false\n- host: api.flowpay.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 26 19:34:00 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: flowpay.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/flowpayio/refs/heads/main/security/flowpayio-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Financing
- Lending
- Embedded Finance
- Fintech
- SME
- Open Banking
- Payments
---
