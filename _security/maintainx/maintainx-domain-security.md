---
api_specs:
- filename: maintainx-openapi-original.json
  format: json
  label: MaintainX REST API v1
  slug: maintainx-rest-api-v1
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/maintainx/refs/heads/main/openapi/maintainx-openapi-original.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: getmaintainx.com
  spf: true
hosts:
- cert_expires: Feb  8 23:59:59 2027 GMT
  host: www.getmaintainx.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Mar 13 23:59:59 2027 GMT
  host: api.getmaintainx.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Maintainx Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for MaintainX, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: MaintainX
provider_slug: maintainx
slug: maintainx-domain-security
source_filename: maintainx-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.getmaintainx.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  8 23:59:59 2027 GMT\n  hsts: false\n- host: api.getmaintainx.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar 13 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: getmaintainx.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/maintainx/refs/heads/main/security/maintainx-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Physical Ai
- Maintenance
- CMMS
- Asset Management
- Work Orders
- Field Service
- Manufacturing
- Preventive Maintenance
- IoT
---
