---
api_specs:
- filename: sense360-openapi-generated.yml
  format: yaml
  label: Sense360 API
  slug: sense360-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/sense360/openapi/_ae-authored/sense360-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: mysense360.com
  spf: true
hosts:
- cert_expires: Nov 30 08:48:03 2026 GMT
  host: mysense360.com
  hsts: true
  hsts_max_age: 7889238
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Sense360 Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Sense360, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Sense360
provider_slug: sense360
slug: sense360-domain-security
source_filename: sense360-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-25'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: mysense360.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 30 08:48:03 2026 GMT\n  hsts: true\n  hsts_max_age: 7889238\ndomains:\n- domain: mysense360.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/sense360/security/sense360-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- HomeAutomation
- IoT
- Sensors
- ESPHome
---
