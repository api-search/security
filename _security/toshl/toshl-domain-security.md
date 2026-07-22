---
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issue "d-trust.net"
  - 0 issue "entrust.net"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: toshl.com
  spf: true
hosts:
- cert_expires: Aug 25 08:04:20 2026 GMT
  host: toshl.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
- cert_expires: Aug 25 08:04:20 2026 GMT
  host: developer.toshl.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
- cert_expires: Aug 25 08:04:20 2026 GMT
  host: api.toshl.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Toshl Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Toshl, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.2); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Toshl
provider_slug: toshl
slug: toshl-domain-security
source_filename: toshl-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: toshl.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Aug 25 08:04:20 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developer.toshl.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Aug 25 08:04:20 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.toshl.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Aug 25 08:04:20 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: toshl.com\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"d-trust.net\"\n  - 0 issue \"entrust.net\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/toshl/refs/heads/main/security/toshl-domain-security.yml
summary_line: TLSv1.2 · HSTS · DMARC
tags:
- Personal Finance
- Budgeting
- Expense Tracking
- FinTech
- Banking
- Consumer Apps
- Company
---
