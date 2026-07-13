---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: youneedabudget.com
  spf: true
hosts:
- cert_expires: Sep  4 15:44:50 2026 GMT
  host: api.youneedabudget.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Ynab Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for YNAB, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: YNAB
provider_slug: ynab
slug: ynab-domain-security
source_filename: ynab-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: api.youneedabudget.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  4 15:44:50 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: youneedabudget.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ynab/refs/heads/main/security/ynab-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Finance
- Public APIs
---
