---
api_specs:
- filename: openapi.json
  format: json
  label: Opentrons HTTP API
  slug: opentrons-http-api
  spec_type: OpenAPI
  url: http://{ROBOT_IP}:31950/openapi.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: opentrons.com
  spf: true
hosts:
- cert_expires: Oct  5 00:04:46 2026 GMT
  host: opentrons.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 18 23:59:59 2026 GMT
  host: docs.opentrons.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Opentrons Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Opentrons, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Opentrons
provider_slug: opentrons
slug: opentrons-domain-security
source_filename: opentrons-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: opentrons.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  5 00:04:46 2026 GMT\n  hsts: false\n- host: docs.opentrons.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 18 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: opentrons.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/opentrons/refs/heads/main/security/opentrons-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Lab Automation
- Liquid Handling
- Robotics
- Biology
- Life Sciences
- Protocol Management
- Hardware Control
- Open Source
---
