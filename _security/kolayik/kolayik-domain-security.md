---
api_specs:
- filename: kolayik-public-api-openapi.yml
  format: yaml
  label: Kolay Public API
  slug: kolay-public-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kolayik/refs/heads/main/openapi/kolayik-public-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: kolayik.com
  spf: true
hosts:
- cert_expires: Sep 25 23:48:17 2026 GMT
  host: kolayik.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  6 06:50:51 2026 GMT
  host: apidocs.kolayik.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 21 11:34:16 2026 GMT
  host: api.kolayik.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Kolayik Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for KolayIK, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: KolayIK
provider_slug: kolayik
slug: kolayik-domain-security
source_filename: kolayik-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: kolayik.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 25 23:48:17 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: apidocs.kolayik.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  6 06:50:51 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.kolayik.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 21 11:34:16 2026 GMT\n  hsts: null\ndomains:\n- domain: kolayik.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/kolayik/refs/heads/main/security/kolayik-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Human Resources
- HR
- Payroll
- Human Capital Management
- Employee Management
- Time and Attendance
- Applicant Tracking
- SaaS
- Turkey
---
