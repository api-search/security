---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: swapi.tech
  spf: true
hosts:
- cert_expires: Sep 21 15:57:50 2026 GMT
  host: www.swapi.tech
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Swapi Swapi Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for SWAPI, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: SWAPI
provider_slug: swapi-swapi
slug: swapi-swapi-domain-security
source_filename: swapi-swapi-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.swapi.tech\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 21 15:57:50 2026 GMT\n  hsts: null\ndomains:\n- domain: swapi.tech\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/swapi-swapi/refs/heads/main/security/swapi-swapi-domain-security.yml
summary_line: TLSv1.3
tags:
- Video
- Public APIs
---
