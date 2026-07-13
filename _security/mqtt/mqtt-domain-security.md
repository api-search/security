---
api_specs:
- filename: asyncapi.yml
  format: yaml
  label: MQTT Version 5.0 Protocol
  slug: protocol-v5
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/mqtt/refs/heads/main/asyncapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: mqtt.org
  spf: false
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: oasis-open.org
  spf: true
hosts:
- cert_expires: Sep 22 20:15:21 2026 GMT
  host: mqtt.org
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  3 09:37:11 2026 GMT
  host: docs.oasis-open.org
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Mqtt Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for MQTT, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: MQTT
provider_slug: mqtt
slug: mqtt-domain-security
source_filename: mqtt-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: mqtt.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 22 20:15:21 2026 GMT\n  hsts: false\n- host: docs.oasis-open.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  3 09:37:11 2026 GMT\n  hsts: false\ndomains:\n- domain: mqtt.org\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n- domain: oasis-open.org\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mqtt/refs/heads/main/security/mqtt-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- MQTT
- Messaging
- Publish Subscribe
- IoT
- M2M
- Protocol
- OASIS Standard
- Telemetry
---
