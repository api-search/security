---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: dezerv.in
  spf: true
hosts:
- cert_expires: Oct 29 23:59:59 2026 GMT
  host: www.dezerv.in
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Dezerv Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Dezerv, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Dezerv
provider_slug: dezerv
slug: dezerv-domain-security
source_filename: dezerv-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.dezerv.in\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 29 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: dezerv.in\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/dezerv/refs/heads/main/security/dezerv-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Services
- Wealth Management
- Investment
- Portfolio Management
- Mutual Funds
- Fintech
- India
- Financial Services
---
