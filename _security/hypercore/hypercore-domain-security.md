---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: hypercore.ai
  spf: true
hosts:
- cert_expires: Sep 28 07:27:10 2026 GMT
  host: www.hypercore.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 21 23:59:59 2026 GMT
  host: docs.hypercore.ai
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  7 23:59:59 2026 GMT
  host: api.hypercore.ai
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Hypercore Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Hypercore, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Hypercore
provider_slug: hypercore
slug: hypercore-domain-security
source_filename: hypercore-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.hypercore.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 28 07:27:10 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.hypercore.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 21 23:59:59 2026 GMT\n  hsts: false\n- host: api.hypercore.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  7 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: hypercore.ai\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hypercore/refs/heads/main/security/hypercore-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Loan Management
- Private Credit
- Lending
- Venture Debt
- Commercial Real Estate
- Loan Servicing
- Fintech
- Financial Services
- GraphQL
---
