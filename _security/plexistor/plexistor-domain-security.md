---
description: ''
domains:
- caa: []
  dmarc: false
  dmarc_policy: null
  dnssec: false
  domain: plexistor.com
  spf: false
hosts:
- cert_not_after: '2026-09-25'
  host: plexistor.com
  hsts: false
  hsts_max_age: null
  https: true
  server: cloudflare
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Plexistor Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Plexistor, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Plexistor
provider_slug: plexistor
slug: plexistor-domain-security
source_filename: plexistor-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: dig + TLS/HTTP HEAD on plexistor.com (legacy marketing host)\nhosts:\n  - host: plexistor.com\n    https: true\n    tls_version: TLSv1.3\n    hsts: false\n    hsts_max_age: null\n    cert_not_after: '2026-09-25'\n    server: cloudflare\ndomains:\n  - domain: plexistor.com\n    dnssec: false\n    caa: []\n    spf: false\n    dmarc: false\n    dmarc_policy: null\nnotes: >-\n  plexistor.com resolves to a Cloudflare-fronted legacy marketing site for the\n  defunct Software-Defined Memory (SDM) product. No API, developer, or mail\n  security posture is published; absence of HSTS/DNSSEC/CAA/SPF/DMARC is\n  recorded as valid probed data.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/plexistor/refs/heads/main/security/plexistor-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- Storage
- Persistent Memory
- Software-Defined Memory
- Data Infrastructure
- Enterprise Storage
- NVDIMM
- Acquired
---
