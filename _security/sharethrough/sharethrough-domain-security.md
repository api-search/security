---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: sharethrough.com
  spf: true
hosts:
- cert_expires: Oct 14 05:18:50 2026 GMT
  host: www.sharethrough.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov  8 23:39:10 2026 GMT
  host: support.sharethrough.com
  hsts: true
  hsts_max_age: 259200
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 27 23:59:59 2026 GMT
  host: publisher-api.sharethrough.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Sharethrough Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Sharethrough, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Sharethrough
provider_slug: sharethrough
slug: sharethrough-domain-security
source_filename: sharethrough-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-12'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.sharethrough.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 14 05:18:50 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: support.sharethrough.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  8 23:39:10 2026 GMT\n  hsts: true\n  hsts_max_age: 259200\n- host: publisher-api.sharethrough.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 27 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: sharethrough.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sharethrough/refs/heads/main/security/sharethrough-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Native Advertising
- Programmatic Advertising
- SSP
- DSP
- OpenRTB
- Ad Exchange
- Header Bidding
- CTV
- Sustainability
---
