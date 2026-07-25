---
api_specs:
- filename: 7shifts-availability-api-openapi.yml
  format: yaml
  label: 7shifts Availability API
  slug: 7shifts-availability-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/7shifts/refs/heads/main/openapi/7shifts-availability-api-openapi.yml
- filename: 7shifts-companies-api-openapi.yml
  format: yaml
  label: 7shifts Companies API
  slug: 7shifts-companies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/7shifts/refs/heads/main/openapi/7shifts-companies-api-openapi.yml
- filename: 7shifts-departments-api-openapi.yml
  format: yaml
  label: 7shifts Departments API
  slug: 7shifts-departments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/7shifts/refs/heads/main/openapi/7shifts-departments-api-openapi.yml
- filename: 7shifts-identity-api-openapi.yml
  format: yaml
  label: 7shifts Identity API
  slug: 7shifts-identity-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/7shifts/refs/heads/main/openapi/7shifts-identity-api-openapi.yml
- filename: 7shifts-locations-api-openapi.yml
  format: yaml
  label: 7shifts Locations API
  slug: 7shifts-locations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/7shifts/refs/heads/main/openapi/7shifts-locations-api-openapi.yml
- filename: 7shifts-oauth-api-openapi.yml
  format: yaml
  label: 7shifts OAuth API
  slug: 7shifts-oauth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/7shifts/refs/heads/main/openapi/7shifts-oauth-api-openapi.yml
- filename: 7shifts-reporting-api-openapi.yml
  format: yaml
  label: 7shifts Reporting API
  slug: 7shifts-reporting-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/7shifts/refs/heads/main/openapi/7shifts-reporting-api-openapi.yml
- filename: 7shifts-roles-api-openapi.yml
  format: yaml
  label: 7shifts Roles API
  slug: 7shifts-roles-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/7shifts/refs/heads/main/openapi/7shifts-roles-api-openapi.yml
- filename: 7shifts-sales-api-openapi.yml
  format: yaml
  label: 7shifts Sales API
  slug: 7shifts-sales-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/7shifts/refs/heads/main/openapi/7shifts-sales-api-openapi.yml
- filename: 7shifts-shifts-api-openapi.yml
  format: yaml
  label: 7shifts Shifts API
  slug: 7shifts-shifts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/7shifts/refs/heads/main/openapi/7shifts-shifts-api-openapi.yml
- filename: 7shifts-time-off-api-openapi.yml
  format: yaml
  label: 7shifts Time Off API
  slug: 7shifts-time-off-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/7shifts/refs/heads/main/openapi/7shifts-time-off-api-openapi.yml
- filename: 7shifts-time-punches-api-openapi.yml
  format: yaml
  label: 7shifts Time Punches API
  slug: 7shifts-time-punches-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/7shifts/refs/heads/main/openapi/7shifts-time-punches-api-openapi.yml
- filename: 7shifts-users-api-openapi.yml
  format: yaml
  label: 7shifts Users API
  slug: 7shifts-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/7shifts/refs/heads/main/openapi/7shifts-users-api-openapi.yml
- filename: 7shifts-wages-api-openapi.yml
  format: yaml
  label: 7shifts Wages API
  slug: 7shifts-wages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/7shifts/refs/heads/main/openapi/7shifts-wages-api-openapi.yml
- filename: 7shifts-webhooks-api-openapi.yml
  format: yaml
  label: 7shifts Webhooks API
  slug: 7shifts-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/7shifts/refs/heads/main/openapi/7shifts-webhooks-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: 7shifts.com
  spf: true
hosts:
- cert_expires: Sep  4 15:14:31 2026 GMT
  host: www.7shifts.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 22 21:05:25 2026 GMT
  host: developers.7shifts.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  4 15:14:31 2026 GMT
  host: api.7shifts.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: 7Shifts Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for 7shifts, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: 7shifts
provider_slug: 7shifts
slug: 7shifts-domain-security
source_filename: 7shifts-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.7shifts.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  4 15:14:31 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: developers.7shifts.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 22 21:05:25 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.7shifts.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  4 15:14:31 2026 GMT\n  hsts: null\ndomains:\n- domain: 7shifts.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/7shifts/refs/heads/main/security/7shifts-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Restaurant
- Scheduling
- Workforce Management
- Employee Scheduling
- Time Tracking
- HRIS
- Labor
---
