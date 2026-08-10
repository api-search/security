---
api_specs:
- filename: wagestream-absences-api-openapi.yml
  format: yaml
  label: Wagestream Absences API
  slug: wagestream-absences-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wagestream/refs/heads/main/openapi/wagestream-absences-api-openapi.yml
- filename: wagestream-employees-api-openapi.yml
  format: yaml
  label: Wagestream Employees API
  slug: wagestream-employees-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wagestream/refs/heads/main/openapi/wagestream-employees-api-openapi.yml
- filename: wagestream-enrollment-api-openapi.yml
  format: yaml
  label: Wagestream Enrollment API
  slug: wagestream-enrollment-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wagestream/refs/heads/main/openapi/wagestream-enrollment-api-openapi.yml
- filename: wagestream-off-cycle-payment-api-openapi.yml
  format: yaml
  label: Wagestream Off Cycle Payment API
  slug: wagestream-off-cycle-payment-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wagestream/refs/heads/main/openapi/wagestream-off-cycle-payment-api-openapi.yml
- filename: wagestream-shifts-api-openapi.yml
  format: yaml
  label: Wagestream Shifts API
  slug: wagestream-shifts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wagestream/refs/heads/main/openapi/wagestream-shifts-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: stream.co
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: wagestream.io
  spf: true
hosts:
- cert_expires: Sep 30 06:57:20 2026 GMT
  host: stream.co
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  1 11:44:32 2026 GMT
  host: connect.stream.co
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 25 23:59:59 2027 GMT
  host: publicapi.wagestream.io
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Wagestream Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Wagestream, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Wagestream
provider_slug: wagestream
slug: wagestream-domain-security
source_filename: wagestream-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-05'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: stream.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 30 06:57:20 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: connect.stream.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  1 11:44:32 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: publicapi.wagestream.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 25 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: stream.co\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: wagestream.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/wagestream/refs/heads/main/security/wagestream-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- financial-wellbeing
- earned-wage-access
- fintech
- payroll
- human-resources
- workforce-management
- time-and-attendance
- employee-benefits
- workplace-savings
- hr-integrations
- b-corp
- united-kingdom
---
