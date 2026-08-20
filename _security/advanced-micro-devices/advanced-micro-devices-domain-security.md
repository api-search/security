---
api_specs:
- filename: advanced-micro-devices-configuration-api-openapi.yml
  format: yaml
  label: Advanced Micro Devices Configuration API
  slug: advanced-micro-devices-configuration-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/advanced-micro-devices/refs/heads/main/openapi/advanced-micro-devices-configuration-api-openapi.yml
- filename: advanced-micro-devices-credits-api-openapi.yml
  format: yaml
  label: Advanced Micro Devices Credits API
  slug: advanced-micro-devices-credits-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/advanced-micro-devices/refs/heads/main/openapi/advanced-micro-devices-credits-api-openapi.yml
- filename: advanced-micro-devices-devices-api-openapi.yml
  format: yaml
  label: Advanced Micro Devices Devices API
  slug: advanced-micro-devices-devices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/advanced-micro-devices/refs/heads/main/openapi/advanced-micro-devices-devices-api-openapi.yml
- filename: advanced-micro-devices-health-api-openapi.yml
  format: yaml
  label: Advanced Micro Devices Health API
  slug: advanced-micro-devices-health-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/advanced-micro-devices/refs/heads/main/openapi/advanced-micro-devices-health-api-openapi.yml
- filename: advanced-micro-devices-instances-api-openapi.yml
  format: yaml
  label: Advanced Micro Devices Instances API
  slug: advanced-micro-devices-instances-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/advanced-micro-devices/refs/heads/main/openapi/advanced-micro-devices-instances-api-openapi.yml
- filename: advanced-micro-devices-models-api-openapi.yml
  format: yaml
  label: Advanced Micro Devices Models API
  slug: advanced-micro-devices-models-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/advanced-micro-devices/refs/heads/main/openapi/advanced-micro-devices-models-api-openapi.yml
- filename: advanced-micro-devices-monitoring-api-openapi.yml
  format: yaml
  label: Advanced Micro Devices Monitoring API
  slug: advanced-micro-devices-monitoring-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/advanced-micro-devices/refs/heads/main/openapi/advanced-micro-devices-monitoring-api-openapi.yml
- filename: advanced-micro-devices-performance-api-openapi.yml
  format: yaml
  label: Advanced Micro Devices Performance API
  slug: advanced-micro-devices-performance-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/advanced-micro-devices/refs/heads/main/openapi/advanced-micro-devices-performance-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: amd.com
  spf: true
hosts:
- cert_expires: Nov 25 23:59:59 2026 GMT
  host: www.amd.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 10 23:59:59 2026 GMT
  host: developer.amd.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- host: api.developer.amd.com
  https: false
kind: domain-security
layout: security
method: probed
name: Advanced Micro Devices Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Advanced Micro Devices, probed live across 3 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Advanced Micro Devices
provider_slug: advanced-micro-devices
slug: advanced-micro-devices-domain-security
source_filename: advanced-micro-devices-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.amd.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 25 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developer.amd.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 10 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.developer.amd.com\n  https: false\ndomains:\n- domain: amd.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/advanced-micro-devices/refs/heads/main/security/advanced-micro-devices-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Artificial Intelligence
- Cloud Computing
- GPU
- HPC
- Machine-Learning
- Semiconductors
- Fortune 500
---
