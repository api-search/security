---
api_specs:
- filename: cvent-registration-openapi.yml
  format: yaml
  label: Cvent Registration REST API
  slug: rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cvent-registration/refs/heads/main/openapi/cvent-registration-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "amazon.com"
  - 0 issue "comodo.com"
  - 0 issue "digicert.com"
  - 0 issue "globalsign.com"
  - 0 issue "letsencrypt.org"
  - 0 issuewild "amazon.com"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: cvent.com
  spf: true
hosts:
- cert_expires: Nov 16 23:59:59 2026 GMT
  host: www.cvent.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan  7 23:59:59 2027 GMT
  host: developers.cvent.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 16 23:59:59 2026 GMT
  host: api-platform.cvent.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Cvent Registration Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Cvent Registration, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Cvent Registration
provider_slug: cvent-registration
slug: cvent-registration-domain-security
source_filename: cvent-registration-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.cvent.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 16 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: developers.cvent.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  7 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api-platform.cvent.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 16 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: cvent.com\n  dnssec: false\n  caa:\n  - 0 issue \"amazon.com\"\n  - 0 issue \"comodo.com\"\n  - 0 issue \"digicert.com\"\n  - 0 issue \"globalsign.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issuewild \"amazon.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cvent-registration/refs/heads/main/security/cvent-registration-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Attendee Management
- Attendees
- Conferences
- Event Management
- Events
- OAuth 2.0
- On-Site Check-In
- Payments
- Registration
- REST API
- Ticketing
- Webhooks
---
