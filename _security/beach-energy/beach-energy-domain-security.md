---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: beachenergy.com.au
  spf: true
hosts:
- cert_expires: Dec 30 14:26:53 2026 GMT
  host: beachenergy.com.au
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Beach Energy Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Beach Energy, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Beach Energy
provider_slug: beach-energy
slug: beach-energy-domain-security
source_filename: beach-energy-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: beachenergy.com.au\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 30 14:26:53 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: beachenergy.com.au\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/beach-energy/refs/heads/main/security/beach-energy-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Energy
- Oil and Gas
- Natural Gas
- Exploration and Production
- Australia
- ASX Listed
- Carbon Capture and Storage
---
