---
api_specs:
- filename: factorial-openapi.yml
  format: yaml
  label: Factorial Developer API
  slug: developer-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/factorial/refs/heads/main/openapi/factorial-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: factorialhr.com
  spf: true
hosts:
- cert_expires: Oct  8 20:46:56 2026 GMT
  host: factorialhr.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 22 22:03:15 2026 GMT
  host: apidoc.factorialhr.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  4 15:01:18 2026 GMT
  host: api.factorialhr.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Factorial Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Factorial, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Factorial
provider_slug: factorial
slug: factorial-domain-security
source_filename: factorial-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: factorialhr.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  8 20:46:56 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: apidoc.factorialhr.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 22 22:03:15 2026 GMT\n  hsts: null\n- host: api.factorialhr.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  4 15:01:18 2026 GMT\n  hsts: null\ndomains:\n- domain: factorialhr.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/factorial/refs/heads/main/security/factorial-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Human Resources
- HRIS
- Employee Management
- Time Tracking
- Payroll
- Time Off
- Performance Management
---
