---
api_specs:
- filename: nine-fives-attenuator-openapi.yml
  format: yaml
  label: Nine Fives Programmable Attenuator API
  slug: nine-fives-programmable-attenuator-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nine-fives/refs/heads/main/openapi/nine-fives-attenuator-openapi.yml
- filename: nine-fives-switch-openapi.yml
  format: yaml
  label: Nine Fives Programmable SPDT Switch API
  slug: nine-fives-programmable-spdt-switch-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nine-fives/refs/heads/main/openapi/nine-fives-switch-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: ninefives.com
  spf: true
hosts:
- cert_expires: Oct  2 16:46:32 2026 GMT
  host: ninefives.com
  hsts: true
  hsts_max_age: 7889238
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 13 01:47:18 2026 GMT
  host: docs.ninefives.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- host: 192.168.0.95
  https: false
kind: domain-security
layout: security
method: probed
name: Nine Fives Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Nine Fives, probed live across 3 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Nine Fives
provider_slug: nine-fives
slug: nine-fives-domain-security
source_filename: nine-fives-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: ninefives.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  2 16:46:32 2026 GMT\n  hsts: true\n  hsts_max_age: 7889238\n- host: docs.ninefives.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 13 01:47:18 2026 GMT\n  hsts: false\n- host: 192.168.0.95\n  https: false\ndomains:\n- domain: ninefives.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/nine-fives/refs/heads/main/security/nine-fives-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- RF Test Equipment
- Test and Measurement
- Hardware
- IoT
- Instrumentation
- Automation
- Aerospace
- Attenuator
- RF Switch
- SCPI
---
