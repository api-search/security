---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: true
  domain: ornadyne.com
  spf: true
hosts:
- cert_expires: Oct 11 01:38:36 2026 GMT
  host: ornadyne.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Ornadyne Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Ornadyne, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC absent.'
provider_name: Ornadyne
provider_slug: ornadyne
slug: ornadyne-domain-security
source_filename: ornadyne-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: ornadyne.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 11 01:38:36 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: ornadyne.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ornadyne/refs/heads/main/security/ornadyne-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC
tags:
- Company
- Drones
- Robotics
- Aerospace
- Defense
- Hard Tech
- UAV
- Surveillance
- Y Combinator
---
