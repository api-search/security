---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: poynt.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: poynt.net
  spf: true
hosts:
- cert_expires: Sep  7 21:53:44 2026 GMT
  host: www.poynt.com
  hsts: true
  hsts_max_age: 3628800
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 16 19:30:19 2026 GMT
  host: docs.poynt.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  8 19:43:06 2026 GMT
  host: services.poynt.net
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Poynt Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Poynt, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Poynt
provider_slug: poynt
slug: poynt-domain-security
source_filename: poynt-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.poynt.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  7 21:53:44 2026 GMT\n  hsts: true\n  hsts_max_age: 3628800\n- host: docs.poynt.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 16 19:30:19 2026 GMT\n  hsts: false\n- host: services.poynt.net\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Sep  8 19:43:06 2026 GMT\n  hsts: null\ndomains:\n- domain: poynt.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: poynt.net\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/poynt/refs/heads/main/security/poynt-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Consumer
- Payments
- Point of Sale
- Commerce
- Merchant Services
- Payment Processing
- Developer Platform
---
