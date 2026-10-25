---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: vivaenergy.com.au
  spf: true
hosts:
- cert_expires: Oct 26 16:30:55 2026 GMT
  host: vivaenergy.com.au
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Viva Energy Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Viva Energy, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Viva Energy
provider_slug: viva-energy
slug: viva-energy-domain-security
source_filename: viva-energy-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-22'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: vivaenergy.com.au\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 26 16:30:55 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: vivaenergy.com.au\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/viva-energy/refs/heads/main/security/viva-energy-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Energy
- Fuel
- Oil and Gas
- Refining
- Retail
- Australia
- Aviation
---
