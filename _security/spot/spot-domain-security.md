---
api_specs:
- filename: spot-devices-openapi.json
  format: json
  label: Spot AI — Devices
  slug: spot-ai-devices
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spot/refs/heads/main/openapi/spot-devices-openapi.json
- filename: spot-intelligence-openapi.json
  format: json
  label: Spot AI — Intelligence
  slug: spot-ai-intelligence
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spot/refs/heads/main/openapi/spot-intelligence-openapi.json
- filename: spot-connect-openapi.json
  format: json
  label: Spot AI — Spot Connect (beta)
  slug: spot-ai-spot-connect-beta
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spot/refs/heads/main/openapi/spot-connect-openapi.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: spot.ai
  spf: true
hosts:
- cert_expires: Sep 28 18:10:06 2026 GMT
  host: www.spot.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 28 22:31:40 2026 GMT
  host: developers.spot.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 31 04:44:12 2026 GMT
  host: dev-api.spot.ai
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Spot Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Spot, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Spot
provider_slug: spot
slug: spot-domain-security
source_filename: spot-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.spot.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 28 18:10:06 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developers.spot.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 28 22:31:40 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: dev-api.spot.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 31 04:44:12 2026 GMT\n  hsts: null\ndomains:\n- domain: spot.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/spot/refs/heads/main/security/spot-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Video
- Physical Security
- Surveillance
- Computer Vision
- Artificial Intelligence
- Cameras
- Analytics
- License Plate Recognition
- Webhooks
- Integrations
---
