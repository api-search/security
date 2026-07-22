---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: qashio.com
  spf: true
hosts:
- cert_expires: Oct 18 22:43:23 2026 GMT
  host: qashio.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Qashio Holding Company Limited Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Qashio Holding Company Limited, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Qashio Holding Company Limited
provider_slug: qashio-holding-company-limited
slug: qashio-holding-company-limited-domain-security
source_filename: qashio-holding-company-limited-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: qashio.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 18 22:43:23 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: qashio.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/qashio-holding-company-limited/refs/heads/main/security/qashio-holding-company-limited-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Fintech
- Corporate Cards
- Spend Management
- Expense Management
- Payments
- United Arab Emirates
---
