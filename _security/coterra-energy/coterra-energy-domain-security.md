---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: coterra.com
  spf: true
hosts:
- cert_expires: Sep 10 15:48:55 2026 GMT
  host: www.coterra.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- host: developer.coterra.com
  https: false
- host: api.coterra.com
  https: false
kind: domain-security
layout: security
method: probed
name: Coterra Energy Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Coterra Energy, probed live across 3 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Coterra Energy
provider_slug: coterra-energy
slug: coterra-energy-domain-security
source_filename: coterra-energy-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.coterra.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 10 15:48:55 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developer.coterra.com\n  https: false\n- host: api.coterra.com\n  https: false\ndomains:\n- domain: coterra.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/coterra-energy/refs/heads/main/security/coterra-energy-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Energy
- Oil and Gas
- Exploration
---
