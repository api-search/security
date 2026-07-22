---
api_specs:
- filename: tank-utility-devices-openapi.yml
  format: yaml
  label: Tank Utility Propane Monitor API
  slug: tank-utility-devices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tank-utility/refs/heads/main/openapi/tank-utility-devices-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: tankutility.com
  spf: true
hosts:
- cert_expires: Sep 20 17:17:13 2026 GMT
  host: tankutility.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 20 17:17:13 2026 GMT
  host: data.tankutility.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Tank Utility Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Tank Utility, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Tank Utility
provider_slug: tank-utility
slug: tank-utility-domain-security
source_filename: tank-utility-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: tankutility.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 20 17:17:13 2026 GMT\n  hsts: false\n- host: data.tankutility.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 20 17:17:13 2026 GMT\n  hsts: null\ndomains:\n- domain: tankutility.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tank-utility/refs/heads/main/security/tank-utility-domain-security.yml
summary_line: TLSv1.3
tags:
- Propane
- Tank Monitoring
- IoT
- Fuel Delivery
- Telemetry
- Energy
- Sensors
- Company
---
