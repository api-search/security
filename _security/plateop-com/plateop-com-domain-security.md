---
api_specs:
- filename: plateop-com-well-known-openapi.json
  format: json
  label: 'Plate-op: publiek voertuigrapport op kenteken .well-known API'
  slug: plate-op-publiek-voertuigrapport-op-kenteken-well-known-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/plateop-com/openapi/_original/plateop-com-well-known-openapi.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: plateop.com
  spf: true
hosts:
- cert_expires: Jan  5 22:55:57 2027 GMT
  host: plateop.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Plateop Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for plateop-com, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: plateop-com
provider_slug: plateop-com
slug: plateop-com-domain-security
source_filename: plateop-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: plateop.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  5 22:55:57 2027 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: plateop.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/plateop-com/security/plateop-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
---
