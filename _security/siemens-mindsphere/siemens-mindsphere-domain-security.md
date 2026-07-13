---
api_specs:
- filename: siemens-mindsphere-asset-management-openapi.yml
  format: yaml
  label: Siemens MindSphere Asset Management API
  slug: asset-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/siemens-mindsphere/refs/heads/main/openapi/siemens-mindsphere-asset-management-openapi.yml
- filename: siemens-mindsphere-iot-timeseries-openapi.yml
  format: yaml
  label: Siemens MindSphere IoT Time Series API
  slug: iot-timeseries-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/siemens-mindsphere/refs/heads/main/openapi/siemens-mindsphere-iot-timeseries-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: siemens.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: mindsphere.io
  spf: true
hosts:
- cert_expires: Feb 13 23:59:59 2027 GMT
  host: siemens.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 18 23:59:59 2026 GMT
  host: documentation.mindsphere.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec  4 23:59:59 2026 GMT
  host: gateway.eu1.mindsphere.io
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Siemens Mindsphere Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Siemens MindSphere, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Siemens MindSphere
provider_slug: siemens-mindsphere
slug: siemens-mindsphere-domain-security
source_filename: siemens-mindsphere-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: siemens.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 13 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: documentation.mindsphere.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 18 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: gateway.eu1.mindsphere.io\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Dec  4 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: siemens.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: mindsphere.io\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/siemens-mindsphere/refs/heads/main/security/siemens-mindsphere-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- IoT
- Industrial
- Digital Twin
- Time Series
- Asset Management
- Industrial IoT
- Insights Hub
---
