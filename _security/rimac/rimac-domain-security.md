---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: rimac-group.com
  spf: true
hosts:
- cert_expires: Sep 22 14:30:06 2026 GMT
  host: www.rimac-group.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Rimac Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Rimac, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Rimac
provider_slug: rimac
slug: rimac-domain-security
source_filename: rimac-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.rimac-group.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 22 14:30:06 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: rimac-group.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/rimac/refs/heads/main/security/rimac-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Transportation
- Electric Vehicles
- Automotive
- Batteries
- Electrification
- Hypercars
- Mobility
---
