---
api_specs:
- filename: packetexchange-io-openapi-generated.yml
  format: yaml
  label: PacketExchange API
  slug: packetexchange-io-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/packetexchange-io/openapi/_ae-authored/packetexchange-io-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: packetexchange.io
  spf: true
hosts:
- cert_expires: Jan 14 17:08:00 2027 GMT
  host: packetexchange.io
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: PacketExchange Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for PacketExchange, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: PacketExchange
provider_slug: packetexchange-io
slug: packetexchange-io-domain-security
source_filename: packetexchange-io-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: packetexchange.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 14 17:08:00 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: packetexchange.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/packetexchange-io/security/packetexchange-io-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Voice
- SMS
- VoIP
- Marketplace
---
