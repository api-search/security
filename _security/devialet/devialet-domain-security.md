---
api_specs:
- filename: devialet-audio-settings-api-openapi.yml
  format: yaml
  label: Devialet Audio Settings API
  slug: devialet-audio-settings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/devialet/refs/heads/main/openapi/devialet-audio-settings-api-openapi.yml
- filename: devialet-devices-api-openapi.yml
  format: yaml
  label: Devialet Devices API
  slug: devialet-devices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/devialet/refs/heads/main/openapi/devialet-devices-api-openapi.yml
- filename: devialet-groups-api-openapi.yml
  format: yaml
  label: Devialet Groups API
  slug: devialet-groups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/devialet/refs/heads/main/openapi/devialet-groups-api-openapi.yml
- filename: devialet-playback-api-openapi.yml
  format: yaml
  label: Devialet Playback API
  slug: devialet-playback-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/devialet/refs/heads/main/openapi/devialet-playback-api-openapi.yml
- filename: devialet-sound-control-api-openapi.yml
  format: yaml
  label: Devialet Sound Control API
  slug: devialet-sound-control-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/devialet/refs/heads/main/openapi/devialet-sound-control-api-openapi.yml
- filename: devialet-systems-api-openapi.yml
  format: yaml
  label: Devialet Systems API
  slug: devialet-systems-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/devialet/refs/heads/main/openapi/devialet-systems-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: devialet.com
  spf: true
hosts:
- cert_expires: Oct  2 11:47:14 2026 GMT
  host: www.devialet.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  9 23:39:06 2026 GMT
  host: help.devialet.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- host: 192.168.1.20
  https: false
kind: domain-security
layout: security
method: probed
name: Devialet Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Devialet, probed live across 3 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Devialet
provider_slug: devialet
slug: devialet-domain-security
source_filename: devialet-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-04'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.devialet.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  2 11:47:14 2026 GMT\n  hsts: null\n- host: help.devialet.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  9 23:39:06 2026 GMT\n  hsts: null\n- host: 192.168.1.20\n  https: false\ndomains:\n- domain: devialet.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/devialet/refs/heads/main/security/devialet-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Audio
- Consumer Electronics
- Smart Speakers
- Home Automation
- Custom Installation
- Device Control
- Local Network API
- IoT
- Hardware
- Music
- France
---
