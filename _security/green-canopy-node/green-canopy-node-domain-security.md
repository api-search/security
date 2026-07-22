---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: greencanopynode.com
  spf: true
hosts:
- cert_expires: Aug 22 15:05:59 2026 GMT
  host: greencanopynode.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Green Canopy Node Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Green Canopy NODE, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Green Canopy NODE
provider_slug: green-canopy-node
slug: green-canopy-node-domain-security
source_filename: green-canopy-node-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: greencanopynode.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 22 15:05:59 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: greencanopynode.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/green-canopy-node/refs/heads/main/security/green-canopy-node-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Real Estate
- Construction Technology
- Sustainability
- Prefab Housing
- Mass Timber
- Impact Investing
- Clean Energy
---
