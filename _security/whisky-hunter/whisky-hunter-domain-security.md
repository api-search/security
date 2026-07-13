---
api_specs:
- filename: whisky-hunter-openapi.yml
  format: yaml
  label: Whisky Hunter API
  slug: whisky-hunter
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/whisky-hunter/refs/heads/main/openapi/whisky-hunter-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: whiskyhunter.net
  spf: true
hosts:
- cert_expires: Oct  5 17:13:40 2026 GMT
  host: whiskyhunter.net
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Whisky Hunter Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Whisky Hunter, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: Whisky Hunter
provider_slug: whisky-hunter
slug: whisky-hunter-domain-security
source_filename: whisky-hunter-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: whiskyhunter.net\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  5 17:13:40 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: whiskyhunter.net\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/whisky-hunter/refs/heads/main/security/whisky-hunter-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Whisky
- Spirits
- Auctions
- Market Data
- Collectors
- Investors
---
