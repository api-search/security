---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: every.io
  spf: true
hosts:
- cert_expires: Sep 12 03:28:00 2026 GMT
  host: www.every.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Every Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Every, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Every
provider_slug: every
slug: every-domain-security
source_filename: every-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.every.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 12 03:28:00 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: every.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/every/refs/heads/main/security/every-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Fintech
- Banking
- Payroll
- HR
- Bookkeeping
- Accounting
- Tax
- Treasury
- Incorporation
- Startups
---
