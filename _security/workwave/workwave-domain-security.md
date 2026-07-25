---
api_specs:
- filename: workwave-callback-api-openapi.yml
  format: yaml
  label: WorkWave Callback API
  slug: workwave-callback-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/workwave/refs/heads/main/openapi/workwave-callback-api-openapi.yml
- filename: workwave-companies-api-openapi.yml
  format: yaml
  label: WorkWave Companies API
  slug: workwave-companies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/workwave/refs/heads/main/openapi/workwave-companies-api-openapi.yml
- filename: workwave-depots-api-openapi.yml
  format: yaml
  label: WorkWave Depots API
  slug: workwave-depots-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/workwave/refs/heads/main/openapi/workwave-depots-api-openapi.yml
- filename: workwave-drivers-api-openapi.yml
  format: yaml
  label: WorkWave Drivers API
  slug: workwave-drivers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/workwave/refs/heads/main/openapi/workwave-drivers-api-openapi.yml
- filename: workwave-gps-api-openapi.yml
  format: yaml
  label: WorkWave GPS API
  slug: workwave-gps-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/workwave/refs/heads/main/openapi/workwave-gps-api-openapi.yml
- filename: workwave-orders-api-openapi.yml
  format: yaml
  label: WorkWave Orders API
  slug: workwave-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/workwave/refs/heads/main/openapi/workwave-orders-api-openapi.yml
- filename: workwave-regions-api-openapi.yml
  format: yaml
  label: WorkWave Regions API
  slug: workwave-regions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/workwave/refs/heads/main/openapi/workwave-regions-api-openapi.yml
- filename: workwave-routes-api-openapi.yml
  format: yaml
  label: WorkWave Routes API
  slug: workwave-routes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/workwave/refs/heads/main/openapi/workwave-routes-api-openapi.yml
- filename: workwave-territories-api-openapi.yml
  format: yaml
  label: WorkWave Territories API
  slug: workwave-territories-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/workwave/refs/heads/main/openapi/workwave-territories-api-openapi.yml
- filename: workwave-validation-api-openapi.yml
  format: yaml
  label: WorkWave Validation API
  slug: workwave-validation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/workwave/refs/heads/main/openapi/workwave-validation-api-openapi.yml
- filename: workwave-vehicles-api-openapi.yml
  format: yaml
  label: WorkWave Vehicles API
  slug: workwave-vehicles-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/workwave/refs/heads/main/openapi/workwave-vehicles-api-openapi.yml
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
