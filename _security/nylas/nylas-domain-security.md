---
api_specs:
- filename: nylas-admin-api-openapi.yml
  format: yaml
  label: Nylas Admin API
  slug: nylas-admin-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nylas/refs/heads/main/openapi/nylas-admin-api-openapi.yml
- filename: nylas-auth-api-openapi.yml
  format: yaml
  label: Nylas Auth API
  slug: nylas-auth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nylas/refs/heads/main/openapi/nylas-auth-api-openapi.yml
- filename: nylas-calendars-api-openapi.yml
  format: yaml
  label: Nylas Calendars API
  slug: nylas-calendars-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nylas/refs/heads/main/openapi/nylas-calendars-api-openapi.yml
- filename: nylas-contacts-api-openapi.yml
  format: yaml
  label: Nylas Contacts API
  slug: nylas-contacts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nylas/refs/heads/main/openapi/nylas-contacts-api-openapi.yml
- filename: nylas-drafts-api-openapi.yml
  format: yaml
  label: Nylas Drafts API
  slug: nylas-drafts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nylas/refs/heads/main/openapi/nylas-drafts-api-openapi.yml
- filename: nylas-events-api-openapi.yml
  format: yaml
  label: Nylas Events API
  slug: nylas-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nylas/refs/heads/main/openapi/nylas-events-api-openapi.yml
- filename: nylas-grants-api-openapi.yml
  format: yaml
  label: Nylas Grants API
  slug: nylas-grants-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nylas/refs/heads/main/openapi/nylas-grants-api-openapi.yml
- filename: nylas-messages-api-openapi.yml
  format: yaml
  label: Nylas Messages API
  slug: nylas-messages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nylas/refs/heads/main/openapi/nylas-messages-api-openapi.yml
- filename: nylas-scheduling-api-openapi.yml
  format: yaml
  label: Nylas Scheduling API
  slug: nylas-scheduling-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nylas/refs/heads/main/openapi/nylas-scheduling-api-openapi.yml
- filename: nylas-threads-api-openapi.yml
  format: yaml
  label: Nylas Threads API
  slug: nylas-threads-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nylas/refs/heads/main/openapi/nylas-threads-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: nylas.com
  spf: true
hosts:
- cert_expires: Sep  4 01:33:30 2026 GMT
  host: www.nylas.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 15 21:08:12 2026 GMT
  host: developer.nylas.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jul 24 21:16:49 2026 GMT
  host: api.us.nylas.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Nylas Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Nylas, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Nylas
provider_slug: nylas
slug: nylas-domain-security
source_filename: nylas-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.nylas.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  4 01:33:30 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\n- host: developer.nylas.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 15 21:08:12 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.us.nylas.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jul 24 21:16:49 2026 GMT\n  hsts: null\ndomains:\n- domain: nylas.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/nylas/refs/heads/main/security/nylas-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Calendar
- Communications
- Contacts
- Email
- Messaging
- Scheduling
---
