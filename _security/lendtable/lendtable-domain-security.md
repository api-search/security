---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: lendtable.com
  spf: true
hosts:
- cert_expires: Sep 18 21:24:58 2026 GMT
  host: lendtable.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Lendtable Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Lendtable, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Lendtable
provider_slug: lendtable
slug: lendtable-domain-security
source_filename: lendtable-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: lendtable.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 18 21:24:58 2026 GMT\n  hsts: null\ndomains:\n- domain: lendtable.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/lendtable/refs/heads/main/security/lendtable-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Financial Services
- Fintech
- Consumer Lending
- Retirement
- 401k
- ESPP
- Employee Benefits
- Personal Finance
- Defunct
---
