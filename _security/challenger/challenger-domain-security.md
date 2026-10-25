---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: challenger.com.au
  spf: true
hosts:
- cert_expires: Jan  6 14:32:41 2027 GMT
  host: challenger.com.au
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Challenger Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Challenger, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Challenger
provider_slug: challenger
slug: challenger-domain-security
source_filename: challenger-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: challenger.com.au\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  6 14:32:41 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: challenger.com.au\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/challenger/refs/heads/main/security/challenger-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Financial Services
- Retirement Income
- Annuities
- Investment Management
- Life Insurance
- Australia
---
