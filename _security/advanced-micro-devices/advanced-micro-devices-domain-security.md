---
api_specs:
- filename: amd-developer-cloud-api-openapi.yml
  format: yaml
  label: AMD Developer Cloud API
  slug: amd-developer-cloud-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/advanced-micro-devices/refs/heads/main/openapi/amd-developer-cloud-api-openapi.yml
- filename: amd-rocm-management-api-openapi.yml
  format: yaml
  label: AMD ROCm API
  slug: amd-rocm-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/advanced-micro-devices/refs/heads/main/openapi/amd-rocm-management-api-openapi.yml
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
- AI
- Cloud Computing
- GPU
- HPC
- Machine Learning
- Semiconductor
- Fortune 500
---
