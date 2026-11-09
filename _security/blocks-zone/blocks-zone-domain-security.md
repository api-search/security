---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: blocks.zone
  spf: false
hosts:
- cert_expires: Jan 17 14:27:38 2027 GMT
  host: blocks.zone
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Blocks Zone Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Blocks, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=none).'
provider_name: Blocks
provider_slug: blocks-zone
slug: blocks-zone-domain-security
source_filename: blocks-zone-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-02'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: blocks.zone\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 17 14:27:38 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: blocks.zone\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/blocks-zone/security/blocks-zone-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Artificial Intelligence
- Fitness
- Training
- Health Tech
- Endurance
---
