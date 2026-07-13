---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: onwater.io
  spf: false
hosts:
- cert_expires: Sep  4 17:04:13 2026 GMT
  host: onwater.io
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Onwater Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for OnWater, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: OnWater
provider_slug: onwater
slug: onwater-domain-security
source_filename: onwater-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: onwater.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  4 17:04:13 2026 GMT\n  hsts: false\ndomains:\n- domain: onwater.io\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/onwater/refs/heads/main/security/onwater-domain-security.yml
summary_line: TLSv1.3
tags:
- Geocoding
- Public APIs
---
