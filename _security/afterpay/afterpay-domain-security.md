---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: afterpay.com
  spf: true
hosts:
- cert_expires: Oct  8 05:01:12 2026 GMT
  host: www.afterpay.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 24 05:05:50 2026 GMT
  host: developers.afterpay.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  8 05:01:12 2026 GMT
  host: api.afterpay.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Afterpay Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Afterpay, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Afterpay
provider_slug: afterpay
slug: afterpay-domain-security
source_filename: afterpay-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.afterpay.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  8 05:01:12 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developers.afterpay.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 24 05:05:50 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.afterpay.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  8 05:01:12 2026 GMT\n  hsts: null\ndomains:\n- domain: afterpay.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/afterpay/refs/heads/main/security/afterpay-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Fintech
- BNPL
- Payments
- Consumer
- Block
---
