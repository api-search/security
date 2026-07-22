---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: delightree.com
  spf: true
hosts:
- cert_expires: Sep 10 15:01:44 2026 GMT
  host: www.delightree.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Delightree Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Delightree, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Delightree
provider_slug: delightree
slug: delightree-domain-security
source_filename: delightree-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.delightree.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 10 15:01:44 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: delightree.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/delightree/refs/heads/main/security/delightree-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Productivity
- Franchise Management
- Franchise Operations
- Task Management
- Training
- Knowledge Base
- SaaS
---
