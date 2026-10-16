---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: corpowerocean.com
  spf: true
hosts:
- cert_expires: Nov 15 01:42:00 2026 GMT
  host: corpowerocean.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Corpowerocean Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Corpowerocean, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Corpowerocean
provider_slug: corpowerocean
slug: corpowerocean-domain-security
source_filename: corpowerocean-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: corpowerocean.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 15 01:42:00 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: corpowerocean.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/corpowerocean/refs/heads/main/security/corpowerocean-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Energy
- WavePower
- Renewable
- Technology
---
