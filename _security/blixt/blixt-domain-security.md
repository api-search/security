---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: blixt.tech
  spf: true
hosts:
- cert_expires: Aug 28 17:09:07 2026 GMT
  host: blixt.tech
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Blixt Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Blixt, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: Blixt
provider_slug: blixt
slug: blixt-domain-security
source_filename: blixt-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: blixt.tech\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 28 17:09:07 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: blixt.tech\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/blixt/refs/heads/main/security/blixt-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Energy
- Power Infrastructure
- Hardware
- Electrical Distribution
- Deep Tech
- Data Centers
---
