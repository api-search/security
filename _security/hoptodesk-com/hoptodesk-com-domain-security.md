---
api_specs:
- filename: hoptodesk-com-openapi-generated.yml
  format: yaml
  label: HopToDesk API
  slug: hoptodesk-com-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hoptodesk-com/openapi/_ae-authored/hoptodesk-com-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: hoptodesk.com
  spf: true
hosts:
- cert_expires: Jan 27 18:35:46 2027 GMT
  host: hoptodesk.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: HopToDesk Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for HopToDesk, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: HopToDesk
provider_slug: hoptodesk-com
slug: hoptodesk-com-domain-security
source_filename: hoptodesk-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: hoptodesk.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 27 18:35:46 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: hoptodesk.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/hoptodesk-com/security/hoptodesk-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Remote Desktop
- Device Management
- Security
- MSP
- Enterprise
---
