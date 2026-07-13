---
api_specs:
- filename: openapi.yml
  format: yaml
  label: TimezoneDB API
  slug: timezonedb-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/timezonedb/refs/heads/main/openapi/openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: timezonedb.com
  spf: true
hosts:
- cert_expires: Oct  6 02:30:55 2026 GMT
  host: timezonedb.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 21 02:17:03 2026 GMT
  host: api.timezonedb.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Timezonedb Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for TimezoneDB, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: TimezoneDB
provider_slug: timezonedb
slug: timezonedb-domain-security
source_filename: timezonedb-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: timezonedb.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  6 02:30:55 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.timezonedb.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 21 02:17:03 2026 GMT\n  hsts: null\ndomains:\n- domain: timezonedb.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/timezonedb/refs/heads/main/security/timezonedb-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Timezone
- Time
- Geographic Coordinates
- DST
- UTC Offset
- Time Conversion
- Location
---
