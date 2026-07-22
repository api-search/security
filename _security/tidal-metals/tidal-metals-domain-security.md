---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: tidalmetals.com
  spf: true
hosts:
- cert_expires: Oct  1 20:48:19 2026 GMT
  host: tidalmetals.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Tidal Metals Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Tidal Metals, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Tidal Metals
provider_slug: tidal-metals
slug: tidal-metals-domain-security
source_filename: tidal-metals-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: tidalmetals.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  1 20:48:19 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: tidalmetals.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tidal-metals/refs/heads/main/security/tidal-metals-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Magnesium
- Critical Minerals
- Materials
- Cleantech
- Decarbonization
- Seawater Extraction
- Deep Tech
---
