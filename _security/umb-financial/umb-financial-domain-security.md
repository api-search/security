---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: umb.com
  spf: true
hosts:
- cert_expires: Oct  1 21:51:13 2026 GMT
  host: www.umb.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Umb Financial Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for UMB Bank, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: UMB Bank
provider_slug: umb-financial
slug: umb-financial-domain-security
source_filename: umb-financial-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-23'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.umb.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  1 21:51:13 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: umb.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/umb-financial/refs/heads/main/security/umb-financial-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Financial-Services
- Banking
- United States
- Open Finance
- Banking as a Service
- Institutional Banking
- Data Aggregation
---
