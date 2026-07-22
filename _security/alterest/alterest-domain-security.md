---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: alterest.co
  spf: true
hosts:
- cert_expires: Oct  1 21:03:30 2026 GMT
  host: alterest.co
  hsts: true
  hsts_max_age: 31556926
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Alterest Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Alterest, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Alterest
provider_slug: alterest
slug: alterest-domain-security
source_filename: alterest-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: alterest.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  1 21:03:30 2026 GMT\n  hsts: true\n  hsts_max_age: 31556926\ndomains:\n- domain: alterest.co\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/alterest/refs/heads/main/security/alterest-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Fintech
- Asset-Based Finance
- Private Credit
- Structured Finance
- Loan Monitoring
- Securitization
- Data Infrastructure
- Verification
---
