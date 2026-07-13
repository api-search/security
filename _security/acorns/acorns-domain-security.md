---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: acorns.com
  spf: true
hosts:
- cert_expires: Dec  5 19:45:11 2026 GMT
  host: www.acorns.com
  hsts: false
  https: true
  tls_version: TLSv1.2
- cert_expires: Jan 18 23:59:59 2027 GMT
  host: developer.acorns.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Acorns Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Acorns, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.2); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Acorns
provider_slug: acorns
slug: acorns-domain-security
source_filename: acorns-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.acorns.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Dec  5 19:45:11 2026 GMT\n  hsts: false\n- host: developer.acorns.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 18 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: acorns.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/acorns/refs/heads/main/security/acorns-domain-security.yml
summary_line: TLSv1.2 · HSTS · DMARC
tags:
- Micro-Investing
- Personal Finance
- Fintech
- Round-Ups
- Robo-Investing
- Retirement
- Savings
- Banking
- Financial Wellness
---
