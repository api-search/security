---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: zippopotam.us
  spf: false
hosts:
- cert_expires: Aug 31 17:45:43 2026 GMT
  host: www.zippopotam.us
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Zippopotam Us Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Zippopotam.us, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Zippopotam.us
provider_slug: zippopotam-us
slug: zippopotam-us-domain-security
source_filename: zippopotam-us-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.zippopotam.us\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 31 17:45:43 2026 GMT\n  hsts: false\ndomains:\n- domain: zippopotam.us\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/zippopotam-us/refs/heads/main/security/zippopotam-us-domain-security.yml
summary_line: TLSv1.3
tags:
- Geocoding
- Public APIs
---
