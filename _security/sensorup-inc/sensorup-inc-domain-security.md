---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: sensorup.com
  spf: true
hosts:
- cert_expires: Dec 16 07:31:29 2026 GMT
  host: www.sensorup.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Sensorup Inc Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for SensorUp Inc., probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: SensorUp Inc.
provider_slug: sensorup-inc
slug: sensorup-inc-domain-security
source_filename: sensorup-inc-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-23'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.sensorup.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 16 07:31:29 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: sensorup.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/sensorup-inc/security/sensorup-inc-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- IoT
- Industrial
- DataPlatform
- Manufacturing
---
