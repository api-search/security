---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: plotbox.com
  spf: true
hosts:
- cert_expires: Sep  4 13:46:42 2026 GMT
  host: plotbox.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Plotbox Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for PlotBox, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: PlotBox
provider_slug: plotbox
slug: plotbox-domain-security
source_filename: plotbox-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: plotbox.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  4 13:46:42 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: plotbox.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/plotbox/refs/heads/main/security/plotbox-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Deathcare
- Cemetery Management
- Funeral Homes
- Crematory
- SaaS
- GIS Mapping
---
