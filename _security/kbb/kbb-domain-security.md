---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: kbb.com
  spf: true
hosts:
- cert_expires: Sep 13 21:48:54 2026 GMT
  host: www.kbb.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 17 23:59:59 2026 GMT
  host: developer.kbb.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 27 16:56:16 2026 GMT
  host: sandbox.api.kbb.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Kbb Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Kelley Blue Book, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Kelley Blue Book
provider_slug: kbb
slug: kbb-domain-security
source_filename: kbb-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.kbb.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 13 21:48:54 2026 GMT\n  hsts: null\n- host: developer.kbb.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 17 23:59:59 2026 GMT\n  hsts: false\n- host: sandbox.api.kbb.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 27 16:56:16 2026 GMT\n  hsts: null\ndomains:\n- domain: kbb.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/kbb/refs/heads/main/security/kbb-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Automotive
- Vehicle Valuation
- Car Pricing
- Trade-In
- Vehicle Data
- Dealer Tools
---
