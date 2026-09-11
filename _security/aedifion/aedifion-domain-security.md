---
api_specs:
- filename: aedifion-openapi.yml
  format: yaml
  label: aedifion HTTP API
  slug: aedifion-http-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aedifion/refs/heads/main/openapi/aedifion-openapi.yml
- filename: aedifion-mqtt-asyncapi.yml
  format: yaml
  label: aedifion MQTT API
  slug: aedifion-mqtt-api
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/aedifion/refs/heads/main/asyncapi/aedifion-mqtt-asyncapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: aedifion.com
  spf: false
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: aedifion.io
  spf: true
hosts:
- cert_expires: Nov 27 10:05:40 2026 GMT
  host: www.aedifion.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 18 08:32:44 2026 GMT
  host: docs.aedifion.io
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 28 00:14:49 2026 GMT
  host: api.aedifion.io
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 3
kind: domain-security
layout: security
method: probed
name: Aedifion Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Aedifion, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=quarantine).'
provider_name: Aedifion
provider_slug: aedifion
slug: aedifion-domain-security
source_filename: aedifion-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-09'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.aedifion.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 27 10:05:40 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.aedifion.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 18 08:32:44 2026 GMT\n  hsts: false\n- host: api.aedifion.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 28 00:14:49 2026 GMT\n  hsts: false\ndomains:\n- domain: aedifion.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: aedifion.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/aedifion/refs/heads/main/security/aedifion-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Building Automation
- Smart Buildings
- Energy Management
- Internet of Things
- Real Estate
- HVAC
- Sustainability
- Time Series
- Analytics
- MQTT
- Building Operations
- ESG
- PropTech
- Germany
---
