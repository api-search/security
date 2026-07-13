---
api_specs:
- filename: datafiniti-api.yml
  format: yaml
  label: Datafiniti API
  slug: datafiniti-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/datafiniti/refs/heads/main/openapi/datafiniti-api.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: datafiniti.co
  spf: true
hosts:
- cert_expires: Aug 16 07:01:49 2026 GMT
  host: www.datafiniti.co
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 28 07:32:00 2026 GMT
  host: docs.datafiniti.co
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  1 23:59:59 2026 GMT
  host: api.datafiniti.co
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Datafiniti Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Datafiniti, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Datafiniti
provider_slug: datafiniti
slug: datafiniti-domain-security
source_filename: datafiniti-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.datafiniti.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 16 07:01:49 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.datafiniti.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 28 07:32:00 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.datafiniti.co\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Oct  1 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: datafiniti.co\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/datafiniti/refs/heads/main/security/datafiniti-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Business Data
- Data Aggregation
- Data as a Service
- People Data
- Product Data
- Property Data
---
