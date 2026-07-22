---
api_specs:
- filename: meter-openapi-original.yml
  format: yaml
  label: Meter Native RESTful API (Meterest)
  slug: meter-native-restful-api-meterest
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/meter/refs/heads/main/openapi/meter-openapi-original.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: meter.io
  spf: true
hosts:
- cert_expires: Sep 15 05:34:35 2026 GMT
  host: www.meter.io
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Meter Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Meter, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Meter
provider_slug: meter
slug: meter-domain-security
source_filename: meter-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.meter.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 15 05:34:35 2026 GMT\n  hsts: false\ndomains:\n- domain: meter.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/meter/refs/heads/main/security/meter-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Blockchain
- Web3
- Cryptocurrency
- Layer-1
- EVM
- Cross-chain Bridge
- Staking
- Developer Tools
---
