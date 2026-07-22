---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: theoremlp.com
  spf: true
hosts:
- cert_expires: Sep 30 04:43:48 2026 GMT
  host: theoremlp.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Theorem Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Theorem, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Theorem
provider_slug: theorem
slug: theorem-domain-security
source_filename: theorem-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: theoremlp.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 30 04:43:48 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: theoremlp.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/theorem/refs/heads/main/security/theorem-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Fintech
- Credit Underwriting
- Machine Learning
- Consumer Lending
- Loan Securitization
- Capital Markets
- Risk Scoring
- Credit Markets
---
