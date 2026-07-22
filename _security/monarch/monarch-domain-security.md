---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: monarchmoney.com
  spf: true
hosts:
- cert_expires: Sep  5 19:00:10 2026 GMT
  host: monarchmoney.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Monarch Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Monarch, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Monarch
provider_slug: monarch
slug: monarch-domain-security
source_filename: monarch-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: monarchmoney.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  5 19:00:10 2026 GMT\n  hsts: null\ndomains:\n- domain: monarchmoney.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/monarch/refs/heads/main/security/monarch-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Personal Finance
- Fintech
- Budgeting
- Money Management
- Financial Planning
- Consumer
---
