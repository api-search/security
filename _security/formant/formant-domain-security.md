---
api_specs:
- filename: formant-admin-api.yaml
  format: yaml
  label: Formant Admin API
  slug: formant-admin-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/formant/refs/heads/main/openapi/formant-admin-api.yaml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: formant.io
  spf: true
hosts:
- cert_expires: Aug 14 02:31:48 2026 GMT
  host: formant.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  2 20:07:13 2026 GMT
  host: docs.formant.io
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Mar  9 23:59:59 2027 GMT
  host: api.formant.io
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Formant Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Formant, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Formant
provider_slug: formant
slug: formant-domain-security
source_filename: formant-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: formant.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 14 02:31:48 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.formant.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  2 20:07:13 2026 GMT\n  hsts: null\n- host: api.formant.io\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Mar  9 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: formant.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/formant/refs/heads/main/security/formant-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Robotics
- Robot Fleet Management
- Teleoperation
- Observability
- Telemetry
- ROS
- ROS2
- Edge Devices
- Physical Operations
- Incident Management
- Industrial AI
- SCADA
- Predictive Maintenance
- Remote Monitoring
- Embedded Devices
---
