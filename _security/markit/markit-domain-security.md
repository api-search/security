---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: markittrade.com
  spf: true
hosts:
- cert_expires: Sep 22 23:02:31 2026 GMT
  host: markittrade.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Markit Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for MarkIt, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: MarkIt
provider_slug: markit
slug: markit-domain-security
source_filename: markit-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: markittrade.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 22 23:02:31 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: markittrade.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/markit/refs/heads/main/security/markit-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Trade Compliance
- Customs
- Tariff Classification
- HS Code
- HTS Code
- Artificial Intelligence
- AI Agents
- International Trade
- Y Combinator
---
