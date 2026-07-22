---
api_specs:
- filename: tano-openapi-original.json
  format: json
  label: Tano Public API
  slug: tano-public-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tano/refs/heads/main/openapi/tano-openapi-original.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: tano.ai
  spf: true
hosts:
- cert_expires: Oct  2 11:51:15 2026 GMT
  host: tano.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Tano Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Tano, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Tano
provider_slug: tano
slug: tano-domain-security
source_filename: tano-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: tano.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  2 11:51:15 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: tano.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tano/refs/heads/main/security/tano-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Influencer Marketing
- Creator Economy
- Marketing
- Advertising
- Artificial Intelligence
- Social Media
- TikTok
- Instagram
- Agent Native
---
