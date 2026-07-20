---
api_specs:
- filename: ecoflow-iot-openapi.yml
  format: yaml
  label: EcoFlow IoT Open Platform
  slug: ecoflow-iot-open-platform
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ecoflow/refs/heads/main/openapi/ecoflow-iot-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: ecoflow.com
  spf: true
hosts:
- cert_expires: Dec  5 23:59:59 2026 GMT
  host: ecoflow.com
  hsts: true
  hsts_max_age: 7889238
  https: true
  tls_version: TLSv1.2
- cert_expires: Dec  5 23:59:59 2026 GMT
  host: developer.ecoflow.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 24 23:59:59 2027 GMT
  host: api.ecoflow.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Ecoflow Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for EcoFlow, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.2); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: EcoFlow
provider_slug: ecoflow
slug: ecoflow-domain-security
source_filename: ecoflow-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: ecoflow.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Dec  5 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 7889238\n- host: developer.ecoflow.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  5 23:59:59 2026 GMT\n  hsts: false\n- host: api.ecoflow.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 24 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: ecoflow.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ecoflow/refs/heads/main/security/ecoflow-domain-security.yml
summary_line: TLSv1.2 · HSTS · DMARC
tags:
- Company
- Technology
- Energy
- Energy Storage
- Portable Power
- IoT
- Smart Home
- Solar
- Developer API
---
