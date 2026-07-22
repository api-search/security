---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: sumutasu.co.jp
  spf: true
hosts:
- cert_expires: Aug 21 01:51:17 2026 GMT
  host: sumutasu.co.jp
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Sumutasu Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Sumutasu, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Sumutasu
provider_slug: sumutasu
slug: sumutasu-domain-security
source_filename: sumutasu-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: sumutasu.co.jp\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 21 01:51:17 2026 GMT\n  hsts: false\ndomains:\n- domain: sumutasu.co.jp\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sumutasu/refs/heads/main/security/sumutasu-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Real Estate
- PropTech
- Japan
- iBuyer
- Housing
- Marketplace
---
