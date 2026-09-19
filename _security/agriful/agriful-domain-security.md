---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: agrifulsoftware.com
  spf: true
hosts:
- cert_expires: Nov 27 03:51:19 2026 GMT
  host: www.agrifulsoftware.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Agriful Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Agriful, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Agriful
provider_slug: agriful
slug: agriful-domain-security
source_filename: agriful-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-12'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.agrifulsoftware.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 27 03:51:19 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: agrifulsoftware.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/agriful/refs/heads/main/security/agriful-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Agriculture
- Fresh Produce
- Food Supply Chain
- Traceability
- ERP
- Inventory Management
- Order Management
- Accounting
- Software-as-a-Service
- Company
---
