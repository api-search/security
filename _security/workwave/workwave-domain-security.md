---
api_specs:
- filename: workwave-openapi.yml
  format: yaml
  label: WorkWave Route Manager - Orders, Routes & Territories
  slug: route-manager-orders-routes
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/workwave/refs/heads/main/openapi/workwave-openapi.yml
- filename: workwave-openapi.yml
  format: yaml
  label: WorkWave Route Manager - Drivers & Vehicles
  slug: route-manager-drivers-vehicles
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/workwave/refs/heads/main/openapi/workwave-openapi.yml
- filename: workwave-openapi.yml
  format: yaml
  label: WorkWave Route Manager - GPS Tracking
  slug: route-manager-gps-tracking
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/workwave/refs/heads/main/openapi/workwave-openapi.yml
- filename: workwave-openapi.yml
  format: yaml
  label: WorkWave Route Manager - Webhooks
  slug: route-manager-webhooks
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/workwave/refs/heads/main/openapi/workwave-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: workwave.com
  spf: true
hosts:
- cert_expires: Aug 17 16:25:29 2026 GMT
  host: www.workwave.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  6 23:59:59 2026 GMT
  host: wwrm.workwave.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Workwave Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for WorkWave, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: WorkWave
provider_slug: workwave
slug: workwave-domain-security
source_filename: workwave-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.workwave.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 17 16:25:29 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: wwrm.workwave.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  6 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: workwave.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/workwave/refs/heads/main/security/workwave-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Field Service
- Route Optimization
- Last Mile Delivery
- Fleet
- GPS Tracking
- Logistics
---
