---
api_specs:
- filename: breathe-hr-openapi.yml
  format: yaml
  label: Breathe HR REST API
  slug: rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/breathe-hr/refs/heads/main/openapi/breathe-hr-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: breathehr.com
  spf: true
hosts:
- cert_expires: Sep 16 05:17:09 2026 GMT
  host: www.breathehr.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 22 23:59:59 2026 GMT
  host: developer.breathehr.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.2
- cert_expires: Dec 22 23:59:59 2026 GMT
  host: api.breathehr.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Breathe Hr Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Breathe HR, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Breathe HR
provider_slug: breathe-hr
slug: breathe-hr-domain-security
source_filename: breathe-hr-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.breathehr.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 16 05:17:09 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developer.breathehr.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Dec 22 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.breathehr.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Dec 22 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: breathehr.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/breathe-hr/refs/heads/main/security/breathe-hr-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- HR
- HRIS
- Human Resources
- Employee Management
- Absence Management
- Holiday Tracking
- SMB
- UK
---
