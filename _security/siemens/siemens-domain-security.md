---
api_specs:
- filename: siemens-building-operations-openapi.yml
  format: yaml
  label: Siemens Building Operations API
  slug: building-operations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/siemens/refs/heads/main/openapi/siemens-building-operations-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: siemens.com
  spf: true
hosts:
- cert_expires: Jan  6 23:59:59 2027 GMT
  host: www.siemens.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 10 23:59:59 2026 GMT
  host: developer.siemens.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 19 23:59:59 2026 GMT
  host: buildingx.siemens.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Siemens Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Siemens, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Siemens
provider_slug: siemens
slug: siemens-domain-security
source_filename: siemens-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.siemens.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  6 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developer.siemens.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 10 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: buildingx.siemens.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 19 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: siemens.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/siemens/refs/heads/main/security/siemens-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Automation
- Electrification
- Industry
- Manufacturing
- Building Automation
- Industrial IoT
- Smart Buildings
- Digital Twin
---
