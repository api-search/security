---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: infillion.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: truex.com
  spf: true
hosts:
- cert_expires: Oct 25 16:23:59 2026 GMT
  host: infillion.com
  hsts: true
  hsts_max_age: 31622400
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb 10 23:59:59 2027 GMT
  host: get.truex.com
  hsts: null
  https: true
  tls_version: TLSv1.2
- cert_expires: Feb 10 23:59:59 2027 GMT
  host: api.truex.com
  hsts: false
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Truex Media Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Truex Media, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Truex Media
provider_slug: truex-media
slug: truex-media-domain-security
source_filename: truex-media-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-12'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: infillion.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 25 16:23:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31622400\n- host: get.truex.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Feb 10 23:59:59 2027 GMT\n  hsts: null\n- host: api.truex.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Feb 10 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: infillion.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: truex.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/truex-media/refs/heads/main/security/truex-media-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Advertising
- AdTech
- Video Advertising
- Connected TV
- Interactive Advertising
- SDK
- Mobile
- Ad Serving
- Reporting
- Attention Measurement
- OTT
---
