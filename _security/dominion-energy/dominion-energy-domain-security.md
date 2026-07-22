---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: dominionenergy.com
  spf: true
hosts:
- cert_expires: Aug  5 17:17:00 2026 GMT
  host: www.dominionenergy.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Dominion Energy Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Dominion Energy, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Dominion Energy
provider_slug: dominion-energy
slug: dominion-energy-domain-security
source_filename: dominion-energy-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.dominionenergy.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug  5 17:17:00 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: dominionenergy.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/dominion-energy/refs/heads/main/security/dominion-energy-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Energy
- Electricity
- Natural Gas
- Utility
- Fortune 500
---
