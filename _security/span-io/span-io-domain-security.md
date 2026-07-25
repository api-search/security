---
api_specs:
- filename: span-ebus-asyncapi.yml
  format: yaml
  label: SPAN eBus MQTT API
  slug: span-ebus-mqtt-api
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/span-io/refs/heads/main/asyncapi/span-ebus-asyncapi.yml
- filename: span-io-auth-api-openapi.yml
  format: yaml
  label: SPAN Auth API
  slug: span-io-auth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/span-io/refs/heads/main/openapi/span-io-auth-api-openapi.yml
- filename: span-io-circuits-api-openapi.yml
  format: yaml
  label: SPAN Circuits API
  slug: span-io-circuits-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/span-io/refs/heads/main/openapi/span-io-circuits-api-openapi.yml
- filename: span-io-islanding-state-api-openapi.yml
  format: yaml
  label: SPAN Islanding State API
  slug: span-io-islanding-state-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/span-io/refs/heads/main/openapi/span-io-islanding-state-api-openapi.yml
- filename: span-io-panel-api-openapi.yml
  format: yaml
  label: SPAN Panel API
  slug: span-io-panel-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/span-io/refs/heads/main/openapi/span-io-panel-api-openapi.yml
- filename: span-io-spaces-api-openapi.yml
  format: yaml
  label: SPAN Spaces API
  slug: span-io-spaces-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/span-io/refs/heads/main/openapi/span-io-spaces-api-openapi.yml
- filename: span-io-status-api-openapi.yml
  format: yaml
  label: SPAN Status API
  slug: span-io-status-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/span-io/refs/heads/main/openapi/span-io-status-api-openapi.yml
- filename: span-io-storage-api-openapi.yml
  format: yaml
  label: SPAN Storage API
  slug: span-io-storage-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/span-io/refs/heads/main/openapi/span-io-storage-api-openapi.yml
- filename: span-io-wifi-api-openapi.yml
  format: yaml
  label: SPAN Wifi API
  slug: span-io-wifi-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/span-io/refs/heads/main/openapi/span-io-wifi-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: span.io
  spf: true
hosts:
- cert_expires: Aug 24 16:11:45 2026 GMT
  host: www.span.io
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Span Io Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for SPAN, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: SPAN
provider_slug: span-io
slug: span-io-domain-security
source_filename: span-io-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.span.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 24 16:11:45 2026 GMT\n  hsts: false\ndomains:\n- domain: span.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/span-io/refs/heads/main/security/span-io-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Energy
- Home Energy
- Electrification
- Smart Panel
- Electrical Panel
- Home Automation
- Solar
- Energy Storage
- EV Charging
- Grid
- Islanding
- Backup Power
- Demand Response
- IoT
- MQTT
- Homie
- Electrification Bus
- On-Premise
---
