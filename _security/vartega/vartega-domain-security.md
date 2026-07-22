---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: vartega.com
  spf: true
hosts:
- cert_expires: Oct  8 18:33:49 2026 GMT
  host: www.vartega.com
  hsts: true
  hsts_max_age: 0
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Vartega Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Vartega, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Vartega
provider_slug: vartega
slug: vartega-domain-security
source_filename: vartega-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.vartega.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  8 18:33:49 2026 GMT\n  hsts: true\n  hsts_max_age: 0\ndomains:\n- domain: vartega.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/vartega/refs/heads/main/security/vartega-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Advanced Materials
- Carbon Fiber
- Recycling
- Sustainability
- Composites
- Manufacturing
---
