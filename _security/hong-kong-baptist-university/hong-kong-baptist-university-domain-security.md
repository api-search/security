---
api_specs:
- filename: openapi.yaml
  format: yaml
  label: HKBU Scholars Pure Web Service API
  slug: pure-research-api
  spec_type: OpenAPI
  url: https://scholars.hkbu.edu.hk/ws/api/openapi.yaml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: hkbu.edu.hk
  spf: true
hosts:
- cert_expires: Nov  1 23:59:59 2026 GMT
  host: www.hkbu.edu.hk
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  5 04:24:50 2026 GMT
  host: scholars.hkbu.edu.hk
  hsts: true
  hsts_max_age: 2592000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 26 23:59:59 2026 GMT
  host: mapp-api.hkbu.edu.hk
  hsts: true
  hsts_max_age: 86400
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Hong Kong Baptist University Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Hong Kong Baptist University, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Hong Kong Baptist University
provider_slug: hong-kong-baptist-university
slug: hong-kong-baptist-university-domain-security
source_filename: hong-kong-baptist-university-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.hkbu.edu.hk\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  1 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: scholars.hkbu.edu.hk\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  5 04:24:50 2026 GMT\n  hsts: true\n  hsts_max_age: 2592000\n- host: mapp-api.hkbu.edu.hk\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 26 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 86400\ndomains:\n- domain: hkbu.edu.hk\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hong-kong-baptist-university/refs/heads/main/security/hong-kong-baptist-university-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Education
- Higher Education
- University
- Research
- Hong Kong
- Pure
- Research Information
---
