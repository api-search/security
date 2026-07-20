---
api_specs:
- filename: enviance-restapi-openapi-original.json
  format: json
  label: Cority Enviance EMS REST API
  slug: enviance-ems-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/enviance/refs/heads/main/openapi/enviance-restapi-openapi-original.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: enviance.com
  spf: true
hosts:
- cert_expires: Jan 16 23:59:59 2027 GMT
  host: api.enviance.com
  hsts: true
  hsts_max_age: 900
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Enviance Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Enviance, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Enviance
provider_slug: enviance
slug: enviance-domain-security
source_filename: enviance-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: api.enviance.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Jan 16 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 900\ndomains:\n- domain: enviance.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/enviance/refs/heads/main/security/enviance-domain-security.yml
summary_line: TLSv1.2 · HSTS · DMARC
tags:
- Company
- Environmental
- Compliance
- EHS
- Sustainability
- Chemical Management
- Regulatory
- SaaS
---
