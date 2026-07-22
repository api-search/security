---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: wasoko.com
  spf: true
hosts:
- cert_expires: Sep 26 04:49:39 2026 GMT
  host: wasoko.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Sokowatch Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Sokowatch / Wasoko, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Sokowatch / Wasoko
provider_slug: sokowatch
slug: sokowatch-domain-security
source_filename: sokowatch-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: wasoko.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 26 04:49:39 2026 GMT\n  hsts: false\ndomains:\n- domain: wasoko.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sokowatch/refs/heads/main/security/sokowatch-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- B2B Commerce
- Informal Retail
- Distribution
- Supply Chain
- Last-Mile Logistics
- FMCG
- Embedded Fintech
- Inventory Credit
- Buy Now Pay Later
- Working Capital
- Mobile Commerce
- Africa
- East Africa
- Kenya
- Egypt
- Financial Inclusion
---
