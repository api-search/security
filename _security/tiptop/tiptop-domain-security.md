---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: tiptop.com
  spf: true
hosts:
- cert_expires: Sep  4 04:00:19 2026 GMT
  host: docs.tiptop.com
  hsts: true
  hsts_max_age: 31556952
  https: true
  tls_version: TLSv1.3
- host: api.tiptop.com
  hsts: null
  https: true
  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: certificate has expired (_ssl.c:1082)'
kind: domain-security
layout: security
method: probed
name: Tiptop Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Tiptop, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Tiptop
provider_slug: tiptop
slug: tiptop-domain-security
source_filename: tiptop-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: docs.tiptop.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  4 04:00:19 2026 GMT\n  hsts: true\n  hsts_max_age: 31556952\n- host: api.tiptop.com\n  https: true\n  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: certificate has\n    expired (_ssl.c:1082)'\n  hsts: null\ndomains:\n- domain: tiptop.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tiptop/refs/heads/main/security/tiptop-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Payments
- FinTech
- Trade-In
- Checkout
- Commerce
- Pay Over Time
---
