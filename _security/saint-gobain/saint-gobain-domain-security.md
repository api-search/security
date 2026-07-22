---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: saint-gobain.com
  spf: true
hosts:
- cert_expires: Aug 24 05:21:55 2026 GMT
  host: www.saint-gobain.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Saint Gobain Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Saint-Gobain, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Saint-Gobain
provider_slug: saint-gobain
slug: saint-gobain-domain-security
source_filename: saint-gobain-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.saint-gobain.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 24 05:21:55 2026 GMT\n  hsts: null\ndomains:\n- domain: saint-gobain.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/saint-gobain/refs/heads/main/security/saint-gobain-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Building Materials
- Construction
- Industrial Manufacturing
- Insulation
- Glass
- Gypsum
- Abrasives
- Mortars
- Roofing
- Sustainable Construction
- CAC 40
- Multinational
---
