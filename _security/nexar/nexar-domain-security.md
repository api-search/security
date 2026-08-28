---
api_specs:
- filename: nexar-virtualcam-openapi.yml
  format: yaml
  label: CityStream VirtualCam API
  slug: virtualcam
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nexar/refs/heads/main/openapi/nexar-virtualcam-openapi.yml
- filename: nexar-livefeed-openapi.yml
  format: yaml
  label: CityStream Live Feed API
  slug: livefeed
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nexar/refs/heads/main/openapi/nexar-livefeed-openapi.yml
- filename: nexar-workzones-openapi.yml
  format: yaml
  label: CityStream Work Zones API
  slug: workzones
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nexar/refs/heads/main/openapi/nexar-workzones-openapi.yml
- filename: nexar-roadinventory-openapi.yml
  format: yaml
  label: CityStream Road Inventory API
  slug: roadinventory
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nexar/refs/heads/main/openapi/nexar-roadinventory-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: nexar-ai.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: getnexar.com
  spf: true
hosts:
- cert_expires: Oct  2 16:18:53 2026 GMT
  host: www.nexar-ai.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan  4 23:59:59 2027 GMT
  host: developer.getnexar.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan  4 23:59:59 2027 GMT
  host: external.getnexar.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  note: 'HSTS observed directly on a POST to /api/virtualcam/v5/frames (403 RBAC: access denied); server istio-envoy behind CloudFront.'
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Nexar Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Nexar, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Nexar
provider_slug: nexar
slug: nexar-domain-security
source_filename: nexar-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-26'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.nexar-ai.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  2 16:18:53 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developer.getnexar.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  4 23:59:59 2027 GMT\n  hsts: false\n- host: external.getnexar.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  4 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n  note: 'HSTS observed directly on a POST to /api/virtualcam/v5/frames (403 RBAC: access denied); server istio-envoy\n    behind CloudFront.'\ndomains:\n- domain: nexar-ai.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: getnexar.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/nexar/refs/heads/main/security/nexar-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Mapping
- Geospatial
- Transportation
- Computer Vision
- Autonomous Vehicles
- Smart Cities
- Imagery
- Road Data
- Machine Learning
---
