---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: mandolin.com
  spf: true
hosts:
- cert_expires: Sep  8 06:06:03 2026 GMT
  host: www.mandolin.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Mandolin Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Mandolin, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Mandolin
provider_slug: mandolin
slug: mandolin-domain-security
source_filename: mandolin-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.mandolin.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  8 06:06:03 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: mandolin.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mandolin/refs/heads/main/security/mandolin-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Applications
- Healthcare
- Pharmaceuticals
- Automation
- Artificial Intelligence
- Specialty Pharmacy
- Revenue Cycle Management
---
