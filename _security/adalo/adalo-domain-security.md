---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: adalo.com
  spf: true
hosts:
- cert_expires: Aug 16 07:42:34 2026 GMT
  host: www.adalo.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 31 19:18:48 2026 GMT
  host: help.adalo.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 24 04:47:00 2026 GMT
  host: api.adalo.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Adalo Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Adalo, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Adalo
provider_slug: adalo
slug: adalo-domain-security
source_filename: adalo-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.adalo.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 16 07:42:34 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: help.adalo.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 31 19:18:48 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.adalo.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 24 04:47:00 2026 GMT\n  hsts: null\ndomains:\n- domain: adalo.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/adalo/refs/heads/main/security/adalo-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- No-Code
- App Builder
- Mobile App Development
- Web App Development
- Low-Code
- Visual Development
---
