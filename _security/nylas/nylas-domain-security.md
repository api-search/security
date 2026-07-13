---
api_specs:
- filename: nylas-openapi.yml
  format: yaml
  label: Nylas API
  slug: nylas-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nylas/refs/heads/main/openapi/nylas-openapi.yml
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
- Communication
- Contacts
- Email
- Messaging
- Scheduling
---
