---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: gosupercritical.com
  spf: true
hosts:
- cert_expires: Sep 16 16:15:59 2026 GMT
  host: gosupercritical.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Supercritical Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Supercritical, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Supercritical
provider_slug: supercritical
slug: supercritical-domain-security
source_filename: supercritical-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: gosupercritical.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 16 16:15:59 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: gosupercritical.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/supercritical/refs/heads/main/security/supercritical-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Carbon Removal
- Durable CDR
- Engineered Carbon Removal
- Carbon Markets
- Climate Tech
- Net Zero
- Biochar
- BECCS
- Enhanced Weathering
- Direct Air Capture
- Woody Biomass Sinking
- Bio-Oil
- Marketplace
- Sustainability
- ESG
---
