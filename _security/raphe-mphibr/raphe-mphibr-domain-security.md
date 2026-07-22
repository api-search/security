---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: raphe.com
  spf: false
hosts:
- cert_expires: Sep 28 20:03:36 2026 GMT
  host: raphe.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Raphe Mphibr Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Raphe Mphibr, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Raphe Mphibr
provider_slug: raphe-mphibr
slug: raphe-mphibr-domain-security
source_filename: raphe-mphibr-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: raphe.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 28 20:03:36 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: raphe.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/raphe-mphibr/refs/heads/main/security/raphe-mphibr-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Aerospace
- Defense
- Drones
- UAV
- Unmanned Aviation
- Manufacturing
- Carbon Fiber
---
