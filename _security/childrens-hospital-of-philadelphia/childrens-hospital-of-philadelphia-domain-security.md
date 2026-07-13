---
api_specs:
- filename: chop-fhir-r4-openapi.yml
  format: yaml
  label: CHOP FHIR R4 API
  slug: chop-fhir-r4-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/childrens-hospital-of-philadelphia/refs/heads/main/openapi/chop-fhir-r4-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: chop.edu
  spf: true
hosts:
- cert_expires: Sep 13 19:13:45 2026 GMT
  host: www.chop.edu
  hsts: true
  hsts_max_age: 1000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 22 23:59:59 2027 GMT
  host: epicnsproxy.chop.edu
  hsts: null
  https: true
  tls_version: TLSv1.2
- cert_expires: Oct 14 23:59:59 2026 GMT
  host: mychop.chop.edu
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Childrens Hospital Of Philadelphia Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Children''s Hospital of Philadelphia, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Children's Hospital of Philadelphia
provider_slug: childrens-hospital-of-philadelphia
slug: childrens-hospital-of-philadelphia-domain-security
source_filename: childrens-hospital-of-philadelphia-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.chop.edu\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 13 19:13:45 2026 GMT\n  hsts: true\n  hsts_max_age: 1000\n- host: epicnsproxy.chop.edu\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Jan 22 23:59:59 2027 GMT\n  hsts: null\n- host: mychop.chop.edu\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Oct 14 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: chop.edu\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/childrens-hospital-of-philadelphia/refs/heads/main/security/childrens-hospital-of-philadelphia-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Healthcare
- Pediatrics
- FHIR
- SMART On FHIR
- Patient Access
- Provider Directory
- CMS Interoperability
- US Core
- Bulk Data
- Research Data
- Open Data
---
