---
api_specs:
- filename: absence-io-absences-api-openapi.yml
  format: yaml
  label: Absence.io Absences API
  slug: absence-io-absences-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/absence-io/refs/heads/main/openapi/absence-io-absences-api-openapi.yml
- filename: absence-io-allowances-api-openapi.yml
  format: yaml
  label: Absence.io Allowances API
  slug: absence-io-allowances-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/absence-io/refs/heads/main/openapi/absence-io-allowances-api-openapi.yml
- filename: absence-io-departments-api-openapi.yml
  format: yaml
  label: Absence.io Departments API
  slug: absence-io-departments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/absence-io/refs/heads/main/openapi/absence-io-departments-api-openapi.yml
- filename: absence-io-locations-api-openapi.yml
  format: yaml
  label: Absence.io Locations API
  slug: absence-io-locations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/absence-io/refs/heads/main/openapi/absence-io-locations-api-openapi.yml
- filename: absence-io-reason-types-api-openapi.yml
  format: yaml
  label: Absence.io Reason Types API
  slug: absence-io-reason-types-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/absence-io/refs/heads/main/openapi/absence-io-reason-types-api-openapi.yml
- filename: absence-io-timespans-api-openapi.yml
  format: yaml
  label: Absence.io Timespans API
  slug: absence-io-timespans-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/absence-io/refs/heads/main/openapi/absence-io-timespans-api-openapi.yml
- filename: absence-io-users-api-openapi.yml
  format: yaml
  label: Absence.io Users API
  slug: absence-io-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/absence-io/refs/heads/main/openapi/absence-io-users-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "digicert.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "sectigo.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: absence.io
  spf: true
hosts:
- cert_expires: Aug 27 11:03:47 2026 GMT
  host: www.absence.io
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug  5 06:27:31 2026 GMT
  host: app.absence.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Absence Io Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Absence.io, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Absence.io
provider_slug: absence-io
slug: absence-io-domain-security
source_filename: absence-io-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.absence.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 27 11:03:47 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: app.absence.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug  5 06:27:31 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: absence.io\n  dnssec: false\n  caa:\n  - 0 issue \"digicert.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"sectigo.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/absence-io/refs/heads/main/security/absence-io-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Absences
- Employees
- Leave Management
- HR
---
