---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: hostplus.com.au
  spf: true
hosts:
- cert_expires: Nov 26 23:59:59 2026 GMT
  host: hostplus.com.au
  hsts: true
  hsts_max_age: 31557600
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Hostplus Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Hostplus, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Hostplus
provider_slug: hostplus
slug: hostplus-domain-security
source_filename: hostplus-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-22'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: hostplus.com.au\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 26 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31557600\ndomains:\n- domain: hostplus.com.au\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hostplus/refs/heads/main/security/hostplus-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Superannuation
- Financial Services
- Retirement
- Pensions
- Investments
- Australia
---
