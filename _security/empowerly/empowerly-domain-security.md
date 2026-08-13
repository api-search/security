---
api_specs:
- filename: empowerly-status-api-openapi.yml
  format: yaml
  label: Empowerly Status API
  slug: empowerly-status-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/empowerly/refs/heads/main/openapi/empowerly-status-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: empowerly.com
  spf: true
hosts:
- cert_expires: Feb 16 23:59:59 2027 GMT
  host: empowerly.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 14 21:22:05 2026 GMT
  host: status.empowerly.com
  hsts: true
  hsts_max_age: 259200
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Empowerly Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Empowerly, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Empowerly
provider_slug: empowerly
slug: empowerly-domain-security
source_filename: empowerly-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-12'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: empowerly.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 16 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: status.empowerly.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 14 21:22:05 2026 GMT\n  hsts: true\n  hsts_max_age: 259200\ndomains:\n- domain: empowerly.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/empowerly/refs/heads/main/security/empowerly-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- education
- edtech
- college-admissions
- counseling
- students
- career-services
- consumer-services
- status-page
---
