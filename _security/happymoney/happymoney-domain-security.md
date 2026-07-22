---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: happymoney.com
  spf: true
hosts:
- cert_expires: Sep 11 04:58:03 2026 GMT
  host: happymoney.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Happymoney Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Happy Money, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Happy Money
provider_slug: happymoney
slug: happymoney-domain-security
source_filename: happymoney-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: happymoney.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Sep 11 04:58:03 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: happymoney.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/happymoney/refs/heads/main/security/happymoney-domain-security.yml
summary_line: TLSv1.2 · HSTS · DMARC
tags:
- Company
- Fintech
- Lending
- Personal Loans
- Debt Consolidation
- Consumer Finance
- Credit Unions
- Financial Services
---
