---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: finda.co.kr
  spf: true
hosts:
- cert_expires: Jan 15 23:59:59 2027 GMT
  host: finda.co.kr
  hsts: false
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Finda Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Finda, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Finda
provider_slug: finda
slug: finda-domain-security
source_filename: finda-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: finda.co.kr\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Jan 15 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: finda.co.kr\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/finda/refs/heads/main/security/finda-domain-security.yml
summary_line: TLSv1.2 · DMARC
tags:
- Company
- Fintech
- Financial Services
- Loans
- Lending
- Loan Comparison
- Personal Finance
- Credit
- South Korea
---
