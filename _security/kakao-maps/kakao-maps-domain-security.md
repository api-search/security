---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: kakao.com
  spf: true
hosts:
- cert_expires: Sep 29 23:59:59 2026 GMT
  host: apis.map.kakao.com
  hsts: true
  hsts_max_age: 15724800
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Kakao Maps Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Kakao Maps, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Kakao Maps
provider_slug: kakao-maps
slug: kakao-maps-domain-security
source_filename: kakao-maps-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: apis.map.kakao.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Sep 29 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 15724800\ndomains:\n- domain: kakao.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/kakao-maps/refs/heads/main/security/kakao-maps-domain-security.yml
summary_line: TLSv1.2 · HSTS · DMARC
tags:
- Geocoding
- Public APIs
---
