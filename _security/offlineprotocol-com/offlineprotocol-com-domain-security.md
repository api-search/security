---
api_specs:
- filename: offlineprotocol-com-openapi-generated.yml
  format: yaml
  label: offlineprotocol-com API
  slug: offlineprotocol-com-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/offlineprotocol-com/openapi/_ae-authored/offlineprotocol-com-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: offlineprotocol.com
  spf: true
hosts:
- cert_expires: Jan 21 13:44:36 2027 GMT
  host: offlineprotocol.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Offlineprotocol Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for offlineprotocol-com, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: offlineprotocol-com
provider_slug: offlineprotocol-com
slug: offlineprotocol-com-domain-security
source_filename: offlineprotocol-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: offlineprotocol.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 21 13:44:36 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: offlineprotocol.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/offlineprotocol-com/security/offlineprotocol-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Coordination
- Offline-First
- Mesh Networking
- IoT
---
