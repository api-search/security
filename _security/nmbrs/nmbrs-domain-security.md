---
api_specs:
- filename: nmbrs-openapi.yml
  format: yaml
  label: Nmbrs Companies API
  slug: nmbrs-companies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nmbrs/refs/heads/main/openapi/nmbrs-openapi.yml
- filename: nmbrs-openapi.yml
  format: yaml
  label: Nmbrs Employees API
  slug: nmbrs-employees-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nmbrs/refs/heads/main/openapi/nmbrs-openapi.yml
- filename: nmbrs-openapi.yml
  format: yaml
  label: Nmbrs Employments API
  slug: nmbrs-employments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nmbrs/refs/heads/main/openapi/nmbrs-openapi.yml
- filename: nmbrs-openapi.yml
  format: yaml
  label: Nmbrs Payroll & Payruns API
  slug: nmbrs-payroll-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nmbrs/refs/heads/main/openapi/nmbrs-openapi.yml
- filename: nmbrs-openapi.yml
  format: yaml
  label: Nmbrs Wage Components API
  slug: nmbrs-wage-components-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nmbrs/refs/heads/main/openapi/nmbrs-openapi.yml
- filename: nmbrs-openapi.yml
  format: yaml
  label: Nmbrs Absences API
  slug: nmbrs-absences-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nmbrs/refs/heads/main/openapi/nmbrs-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: nmbrs.com
  spf: true
  spf_policy: -all
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: nmbrsapp.com
  spf: true
  spf_policy: ~all
hosts:
- cert_expires: Dec 10 00:39:30 2026 GMT
  host: nmbrs.com
  hsts: true
  hsts_max_age: 31536000
  https: true
- cert_expires: Dec 17 13:25:49 2026 GMT
  host: api.nmbrsapp.com
  hsts: true
  hsts_max_age: 31536000
  hsts_preload: true
  https: true
  note: Current REST API host. GET /api/companies returns 401 unauthenticated.
- cert_expires: Jan  9 14:28:59 2027 GMT
  host: api.nmbrs.nl
  hsts: true
  hsts_max_age: 31536000
  https: true
  note: Legacy SOAP v3 host (deprecated, retiring 2027-03-01).
- cert_expires: Dec 10 00:39:30 2026 GMT
  host: developer.nmbrs.com
  hsts: true
  hsts_max_age: 31536000
  https: true
- cert_expires: Dec 10 00:39:30 2026 GMT
  host: identityservice.nmbrs.com
  hsts: true
  hsts_max_age: 2592000
  https: true
  note: OAuth 2.0 authorization/token endpoints.
kind: domain-security
layout: security
method: probed
name: Nmbrs Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Nmbrs, probed live across 5 host(s) and 2 registrable domain(s). 5 host(s) serve HTTPS; 5 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Nmbrs
provider_slug: nmbrs
slug: nmbrs-domain-security
source_filename: nmbrs-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: nmbrs.com\n  https: true\n  cert_expires: Dec 10 00:39:30 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.nmbrsapp.com\n  https: true\n  cert_expires: Dec 17 13:25:49 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n  hsts_preload: true\n  note: Current REST API host. GET /api/companies returns 401 unauthenticated.\n- host: api.nmbrs.nl\n  https: true\n  cert_expires: Jan  9 14:28:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n  note: Legacy SOAP v3 host (deprecated, retiring 2027-03-01).\n- host: developer.nmbrs.com\n  https: true\n  cert_expires: Dec 10 00:39:30 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: identityservice.nmbrs.com\n  https: true\n  cert_expires: Dec 10 00:39:30 2026 GMT\n  hsts: true\n  hsts_max_age: 2592000\n  note: OAuth 2.0 authorization/token endpoints.\ndomains:\n- domain: nmbrs.com\n  dnssec: false\n\
  \  caa: []\n  spf: true\n  spf_policy: -all\n  dmarc: true\n  dmarc_policy: none\n- domain: nmbrsapp.com\n  dnssec: false\n  caa: []\n  spf: true\n  spf_policy: ~all\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/nmbrs/refs/heads/main/security/nmbrs-domain-security.yml
summary_line: HSTS · DMARC
tags:
- Human Resources
- HRIS
- Payroll
- Employee Management
- HR
- Absence Management
- Netherlands
- Sweden
- SOAP
- REST
---
