---
api_specs:
- filename: d-tools-cloud-api-openapi.yml
  format: yaml
  label: D-Tools Cloud API
  slug: d-tools-cloud-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/d-tools/refs/heads/main/openapi/d-tools-cloud-api-openapi.yml
- filename: d-tools-si-api-openapi.yml
  format: yaml
  label: D-Tools System Integrator (SI) API
  slug: d-tools-system-integrator-si-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/d-tools/refs/heads/main/openapi/d-tools-si-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: d-tools.com
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: d-tools.cloud
  spf: false
hosts:
- cert_expires: Sep 14 18:07:55 2026 GMT
  host: www.d-tools.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Mar  4 06:07:24 2027 GMT
  host: dtcloudapi.d-tools.cloud
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb 12 23:59:59 2027 GMT
  host: api.d-tools.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: D Tools Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for D-Tools, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: D-Tools
provider_slug: d-tools
slug: d-tools-domain-security
source_filename: d-tools-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.d-tools.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 14 18:07:55 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: dtcloudapi.d-tools.cloud\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar  4 06:07:24 2027 GMT\n  hsts: null\n- host: api.d-tools.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 12 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: d-tools.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: d-tools.cloud\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/d-tools/refs/heads/main/security/d-tools-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- av-integration
- Systems Integration
- Project Management
- Estimation
- Quoting
- Field Service Management
- Construction Tech
- low-voltage
- Product Catalog
- ERP Integration
- Vertical SaaS
---
