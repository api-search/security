---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: bunch.capital
  spf: true
hosts:
- cert_expires: Sep 30 10:55:46 2026 GMT
  host: www.bunch.capital
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Bunch Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Bunch, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Bunch
provider_slug: bunch
slug: bunch-domain-security
source_filename: bunch-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.bunch.capital\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 30 10:55:46 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: bunch.capital\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bunch/refs/heads/main/security/bunch-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Fintech
- Private Markets
- Fund Administration
- Fund Operations
- Venture Capital
- Private Equity
- SPV
---
