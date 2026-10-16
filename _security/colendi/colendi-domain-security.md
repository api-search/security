---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: colendi.com
  spf: true
hosts:
- cert_expires: Oct 15 23:59:59 2026 GMT
  host: www.colendi.com
  hsts: true
  hsts_max_age: 5184000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Colendi Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Colendi, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Colendi
provider_slug: colendi
slug: colendi-domain-security
source_filename: colendi-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-09'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.colendi.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 15 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 5184000\ndomains:\n- domain: colendi.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/colendi/refs/heads/main/security/colendi-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Fintech
- EmbeddedFinance
- API
- B2B
- FinancialInclusion
- Company
---
