---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: 4rsystems.com
  spf: true
hosts:
- cert_expires: Nov 13 14:35:38 2026 GMT
  host: 4rsystems.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: 4R Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for 4R Systems, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: 4R Systems
provider_slug: 4r
slug: 4r-domain-security
source_filename: 4r-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-05'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: 4rsystems.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 13 14:35:38 2026 GMT\n  hsts: false\ndomains:\n- domain: 4rsystems.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/4r/refs/heads/main/security/4r-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Retail
- Supply Chain
- Inventory Optimization
- Demand Planning
- Analytics
- Artificial Intelligence
- SaaS
---
