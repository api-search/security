---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: zionsbank.com
  spf: true
hosts:
- cert_expires: Dec 17 23:59:59 2026 GMT
  host: www.zionsbank.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 14 23:59:59 2026 GMT
  host: treasurygateway.zionsbank.com
  hsts: true
  hsts_max_age: 3153600
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Zions Bancorp Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Zions Bancorporation, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Zions Bancorporation
provider_slug: zions-bancorp
slug: zions-bancorp-domain-security
source_filename: zions-bancorp-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.zionsbank.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 17 23:59:59 2026 GMT\n  hsts: null\n- host: treasurygateway.zionsbank.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 14 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 3153600\ndomains:\n- domain: zionsbank.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/zions-bancorp/refs/heads/main/security/zions-bancorp-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Banking
- Financial Services
- Treasury Management
- Payments
- Fortune 1000
---
