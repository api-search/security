---
api_specs:
- filename: packet-guru-connection-api-openapi.yml
  format: yaml
  label: Packet Guru Connection API
  slug: packet-guru-connection-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/packet-guru/openapi/packet-guru-connection-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: packet.guru
  spf: true
hosts:
- cert_expires: Feb  8 08:37:21 2027 GMT
  host: packet.guru
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Packet Guru Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Packet Guru, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Packet Guru
provider_slug: packet-guru
slug: packet-guru-domain-security
source_filename: packet-guru-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: packet.guru\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  8 08:37:21 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: packet.guru\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/packet-guru/security/packet-guru-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Network Tools
- Privacy
- Security
- Utilities
- Open Source
---
