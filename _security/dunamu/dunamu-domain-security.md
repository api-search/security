---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: dunamu.com
  spf: true
hosts:
- cert_expires: Oct  2 23:59:59 2026 GMT
  host: dunamu.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Dunamu Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Dunamu, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Dunamu
provider_slug: dunamu
slug: dunamu-domain-security
source_filename: dunamu-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-12'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: dunamu.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  2 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: dunamu.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/dunamu/refs/heads/main/security/dunamu-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Fintech
- Cryptocurrency
- Digital Assets
- Exchange
- Securities
- Trading
- Blockchain
- South Korea
- Company
---
