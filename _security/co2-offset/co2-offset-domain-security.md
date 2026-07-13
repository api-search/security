---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: co2offset.io
  spf: false
hosts:
- cert_expires: Sep  1 20:35:05 2026 GMT
  host: co2offset.io
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Co2 Offset Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for CO2 Offset, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: CO2 Offset
provider_slug: co2-offset
slug: co2-offset-domain-security
source_filename: co2-offset-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: co2offset.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  1 20:35:05 2026 GMT\n  hsts: false\ndomains:\n- domain: co2offset.io\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/co2-offset/refs/heads/main/security/co2-offset-domain-security.yml
summary_line: TLSv1.3
tags:
- Environment
- Public APIs
---
