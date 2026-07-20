---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: desmos.com
  spf: true
hosts:
- cert_expires: Dec 17 23:59:59 2026 GMT
  host: desmos.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Desmos Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Desmos, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Desmos
provider_slug: desmos
slug: desmos-domain-security
source_filename: desmos-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: desmos.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 17 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: desmos.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/desmos/refs/heads/main/security/desmos-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Consumer
- Education
- Mathematics
- Graphing Calculator
- Embeddable
- JavaScript
- EdTech
- Data Visualization
---
