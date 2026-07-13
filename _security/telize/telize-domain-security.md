---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: true
  domain: rapidapi.com
  spf: true
hosts:
- cert_expires: Sep 18 08:42:50 2026 GMT
  host: rapidapi.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Telize Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Telize, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC absent.'
provider_name: Telize
provider_slug: telize
slug: telize-domain-security
source_filename: telize-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: rapidapi.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 18 08:42:50 2026 GMT\n  hsts: null\ndomains:\n- domain: rapidapi.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/telize/refs/heads/main/security/telize-domain-security.yml
summary_line: TLSv1.3 · DNSSEC
tags:
- Geocoding
- Public APIs
---
