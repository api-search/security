---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: zainartech.com
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: zainar.net
  spf: false
hosts:
- cert_expires: Sep  1 17:37:10 2026 GMT
  host: zainartech.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan  6 23:59:59 2027 GMT
  host: api.wifi-prd-us.zainar.net
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Zainar Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for ZaiNar, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: ZaiNar
provider_slug: zainar
slug: zainar-domain-security
source_filename: zainar-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-02'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: zainartech.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  1 17:37:10 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.wifi-prd-us.zainar.net\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Jan  6 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: zainartech.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: zainar.net\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/zainar/refs/heads/main/security/zainar-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Location
- Positioning
- Navigation
- Timing
- Wireless
- Real-Time Location
- Asset Tracking
- IoT
- Physical AI
---
