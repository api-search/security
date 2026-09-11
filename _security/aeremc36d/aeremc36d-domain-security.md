---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: aerem.co
  spf: true
hosts:
- cert_expires: Nov  5 22:42:53 2026 GMT
  host: www.aerem.co
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Aeremc36D Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Aerem, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Aerem
provider_slug: aeremc36d
slug: aeremc36d-domain-security
source_filename: aeremc36d-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-10'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.aerem.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  5 22:42:53 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: aerem.co\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/aeremc36d/refs/heads/main/security/aeremc36d-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Financial Services
- Lending
- Energy
- Solar
- Clean Energy
- Fintech
- Marketplace
- India
- Non-Banking Financial Company
---
