---
api_specs:
- filename: sea-machines-openapi.yml
  format: yaml
  label: SMLink Streaming-API
  slug: smlink-streaming-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sea-machines/refs/heads/main/openapi/sea-machines-openapi.yml
- filename: sea-machines-openapi.yml
  format: yaml
  label: SMLink Control-API
  slug: smlink-control-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sea-machines/refs/heads/main/openapi/sea-machines-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: sea-machines.com
  spf: true
hosts:
- cert_expires: Aug 12 17:01:37 2026 GMT
  host: sea-machines.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Sea Machines Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Sea Machines Robotics, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Sea Machines Robotics
provider_slug: sea-machines
slug: sea-machines-domain-security
source_filename: sea-machines-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: sea-machines.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 12 17:01:37 2026 GMT\n  hsts: false\ndomains:\n- domain: sea-machines.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sea-machines/refs/heads/main/security/sea-machines-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Marine
- Autonomy
- Robotics
- Maritime
- Computer Vision
- Telemetry
---
