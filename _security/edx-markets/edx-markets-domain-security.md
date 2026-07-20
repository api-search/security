---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: edxmarkets.com
  spf: true
hosts:
- cert_expires: Sep 14 11:29:14 2026 GMT
  host: www.edxmarkets.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Edx Markets Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for EDX Markets, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: EDX Markets
provider_slug: edx-markets
slug: edx-markets-domain-security
source_filename: edx-markets-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.edxmarkets.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 14 11:29:14 2026 GMT\n  hsts: false\ndomains:\n- domain: edxmarkets.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/edx-markets/refs/heads/main/security/edx-markets-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Crypto
- Cryptocurrency
- Digital Assets
- Exchange
- Trading
- FIX Protocol
- Market Data
- Clearing
- Institutional
---
