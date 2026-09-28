---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: betpawa.com
  spf: true
hosts:
- cert_expires: Nov 24 22:17:34 2026 GMT
  host: www.betpawa.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Betpawa Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for BetPawa, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: BetPawa
provider_slug: betpawa
slug: betpawa-domain-security
source_filename: betpawa-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-28'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.betpawa.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 24 22:17:34 2026 GMT\n  hsts: false\ndomains:\n- domain: betpawa.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/betpawa/refs/heads/main/security/betpawa-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Betting
- Sports
- Gaming
- Africa
- Online
---
