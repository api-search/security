---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: varomoney.com
  spf: true
hosts:
- cert_expires: Sep 11 20:28:30 2026 GMT
  host: www.varomoney.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 11 20:28:30 2026 GMT
  host: api.varomoney.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Varo Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Varo Bank, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Varo Bank
provider_slug: varo
slug: varo-domain-security
source_filename: varo-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.varomoney.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 11 20:28:30 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.varomoney.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 11 20:28:30 2026 GMT\n  hsts: null\ndomains:\n- domain: varomoney.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/varo/refs/heads/main/security/varo-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Banking
- Fintech
- Consumer Finance
- Savings
- Cash Advance
- Credit Builder
- Open Banking
- Mobile Banking
- Digital Bank
---
