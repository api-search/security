---
api_specs:
- filename: channelape-openapi-generated.yml
  format: yaml
  label: ChannelApe API
  slug: channelape-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/channelape/refs/heads/main/openapi/_ae-authored/channelape-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: channelape.com
  spf: true
hosts:
- cert_expires: Dec 23 19:01:53 2026 GMT
  host: www.channelape.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Channelape Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for ChannelApe, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: ChannelApe
provider_slug: channelape
slug: channelape-domain-security
source_filename: channelape-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-08'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.channelape.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 23 19:01:53 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: channelape.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/channelape/refs/heads/main/security/channelape-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Inventory
- Operations
- Wholesale
- Retail
- API
---
