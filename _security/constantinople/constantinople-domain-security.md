---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: cxnpl.com
  spf: true
hosts:
- cert_expires: Aug 26 20:42:30 2026 GMT
  host: cxnpl.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Constantinople Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Constantinople, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Constantinople
provider_slug: constantinople
slug: constantinople-domain-security
source_filename: constantinople-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: cxnpl.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 26 20:42:30 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: cxnpl.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/constantinople/refs/heads/main/security/constantinople-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Fintech
- Banking
- Core Banking
- Banking as a Service
- Embedded Finance
- Payments
- Lending
---
