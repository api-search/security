---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: tryalchemize.com
  spf: true
hosts:
- cert_expires: Aug 22 05:57:10 2026 GMT
  host: tryalchemize.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 24 03:05:06 2026 GMT
  host: api.tryalchemize.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Alchemize Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Alchemize, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Alchemize
provider_slug: alchemize
slug: alchemize-domain-security
source_filename: alchemize-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: tryalchemize.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 22 05:57:10 2026 GMT\n  hsts: false\n- host: api.tryalchemize.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 24 03:05:06 2026 GMT\n  hsts: null\ndomains:\n- domain: tryalchemize.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/alchemize/refs/heads/main/security/alchemize-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Customs Brokerage
- Trade Compliance
- Supply Chain
- Logistics
- Import Export
- Artificial Intelligence
- EDI
- Y Combinator
---
