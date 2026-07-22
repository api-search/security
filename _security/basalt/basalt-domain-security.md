---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: true
  domain: basalt.space
  spf: false
hosts:
- cert_expires: Oct 14 20:14:43 2026 GMT
  host: basalt.space
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Basalt Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Basalt, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF absent, DMARC absent.'
provider_name: Basalt
provider_slug: basalt
slug: basalt-domain-security
source_filename: basalt-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: basalt.space\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 14 20:14:43 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: basalt.space\n  dnssec: true\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/basalt/refs/heads/main/security/basalt-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC
tags:
- Company
- Frontier Tech
- Space
- Satellites
- Spacecraft OS
- Aerospace
- Defense
- National Security
---
