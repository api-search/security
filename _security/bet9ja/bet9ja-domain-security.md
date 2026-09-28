---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: bet9ja.com
  spf: true
hosts:
- cert_expires: Mar 13 23:59:59 2027 GMT
  host: bet9ja.com
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Bet9Ja Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Bet9ja, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Bet9ja
provider_slug: bet9ja
slug: bet9ja-domain-security
source_filename: bet9ja-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-28'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: bet9ja.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar 13 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: bet9ja.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bet9ja/refs/heads/main/security/bet9ja-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Sports Betting
- Gaming
- Nigeria
- Online Platform
---
