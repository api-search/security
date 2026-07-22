---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: sourceday.com
  spf: true
hosts:
- cert_expires: Sep 15 05:42:20 2026 GMT
  host: sourceday.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Sourceday Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Sourceday, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Sourceday
provider_slug: sourceday
slug: sourceday-domain-security
source_filename: sourceday-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: sourceday.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 15 05:42:20 2026 GMT\n  hsts: false\ndomains:\n- domain: sourceday.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sourceday/refs/heads/main/security/sourceday-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Supply Chain
- Purchase Orders
- Supplier Management
- Procurement
- ERP Integration
- Manufacturing
- SaaS
---
