---
api_specs:
- filename: tablecheck-availability-api-openapi.yml
  format: yaml
  label: TableCheck availability API
  slug: tablecheck-availability-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tablecheck/refs/heads/main/openapi/tablecheck-availability-api-openapi.yml
- filename: tablecheck-blockages-api-openapi.yml
  format: yaml
  label: TableCheck blockages API
  slug: tablecheck-blockages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tablecheck/refs/heads/main/openapi/tablecheck-blockages-api-openapi.yml
- filename: tablecheck-calendar-api-openapi.yml
  format: yaml
  label: TableCheck calendar API
  slug: tablecheck-calendar-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tablecheck/refs/heads/main/openapi/tablecheck-calendar-api-openapi.yml
- filename: tablecheck-customers-api-openapi.yml
  format: yaml
  label: TableCheck customers API
  slug: tablecheck-customers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tablecheck/refs/heads/main/openapi/tablecheck-customers-api-openapi.yml
- filename: tablecheck-franchises-api-openapi.yml
  format: yaml
  label: TableCheck franchises API
  slug: tablecheck-franchises-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tablecheck/refs/heads/main/openapi/tablecheck-franchises-api-openapi.yml
- filename: tablecheck-membership-programs-api-openapi.yml
  format: yaml
  label: TableCheck membership_programs API
  slug: tablecheck-membership-programs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tablecheck/refs/heads/main/openapi/tablecheck-membership-programs-api-openapi.yml
- filename: tablecheck-memberships-api-openapi.yml
  format: yaml
  label: TableCheck memberships API
  slug: tablecheck-memberships-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tablecheck/refs/heads/main/openapi/tablecheck-memberships-api-openapi.yml
- filename: tablecheck-pos-journals-api-openapi.yml
  format: yaml
  label: TableCheck pos_journals API
  slug: tablecheck-pos-journals-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tablecheck/refs/heads/main/openapi/tablecheck-pos-journals-api-openapi.yml
- filename: tablecheck-reservation-flags-api-openapi.yml
  format: yaml
  label: TableCheck reservation_flags API
  slug: tablecheck-reservation-flags-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tablecheck/refs/heads/main/openapi/tablecheck-reservation-flags-api-openapi.yml
- filename: tablecheck-reservations-api-openapi.yml
  format: yaml
  label: TableCheck reservations API
  slug: tablecheck-reservations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tablecheck/refs/heads/main/openapi/tablecheck-reservations-api-openapi.yml
- filename: tablecheck-shops-api-openapi.yml
  format: yaml
  label: TableCheck shops API
  slug: tablecheck-shops-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tablecheck/refs/heads/main/openapi/tablecheck-shops-api-openapi.yml
- filename: tablecheck-table-status-api-openapi.yml
  format: yaml
  label: TableCheck table_status API
  slug: tablecheck-table-status-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tablecheck/refs/heads/main/openapi/tablecheck-table-status-api-openapi.yml
- filename: tablecheck-tables-api-openapi.yml
  format: yaml
  label: TableCheck tables API
  slug: tablecheck-tables-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tablecheck/refs/heads/main/openapi/tablecheck-tables-api-openapi.yml
- filename: tablecheck-timetable-api-openapi.yml
  format: yaml
  label: TableCheck timetable API
  slug: tablecheck-timetable-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tablecheck/refs/heads/main/openapi/tablecheck-timetable-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issue "sectigo.com"
  - 0 issuewild "amazon.com"
  - 0 issuewild "amazonaws.com"
  - 0 issuewild "amazontrust.com"
  - 0 issuewild "awstrust.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: tablecheck.com
  spf: true
- caa:
  - 0 issuewild "digicert.com; account=c2eb0f50ca113d7543d58a10f523d0469ff922f115e5e4e9056f3d5f87d3356c"
  - 0 issue "amazon.com"
  - 0 issue "digicert.com; account=c2eb0f50ca113d7543d58a10f523d0469ff922f115e5e4e9056f3d5f87d3356c"
  - 0 issuewild "amazon.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: atlassian.net
  spf: true
hosts:
- cert_expires: Dec 22 23:59:59 2026 GMT
  host: www.tablecheck.com
  hsts: true
  hsts_max_age: 31449600
  https: true
  tls_version: TLSv1.2
- cert_expires: Oct  8 23:59:59 2026 GMT
  host: tablecheck.atlassian.net
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 22 23:59:59 2026 GMT
  host: api.tablecheck.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Tablecheck Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for TableCheck, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.2); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: TableCheck
provider_slug: tablecheck
slug: tablecheck-domain-security
source_filename: tablecheck-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.tablecheck.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Dec 22 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31449600\n- host: tablecheck.atlassian.net\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  8 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.tablecheck.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 22 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: tablecheck.com\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"sectigo.com\"\n  - 0 issuewild \"amazon.com\"\n  - 0 issuewild \"amazonaws.com\"\n  - 0 issuewild \"amazontrust.com\"\n  - 0 issuewild \"awstrust.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: atlassian.net\n  dnssec: false\n  caa:\n  - 0 issuewild \"digicert.com; account=c2eb0f50ca113d7543d58a10f523d0469ff922f115e5e4e9056f3d5f87d3356c\"\
  \n  - 0 issue \"amazon.com\"\n  - 0 issue \"digicert.com; account=c2eb0f50ca113d7543d58a10f523d0469ff922f115e5e4e9056f3d5f87d3356c\"\n  - 0 issuewild \"amazon.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tablecheck/refs/heads/main/security/tablecheck-domain-security.yml
summary_line: TLSv1.2 · HSTS · DMARC
tags:
- Restaurant
- Reservations
- Booking
- Hospitality
- Availability
- Guest CRM
- Point of Sale
- Japan
---
