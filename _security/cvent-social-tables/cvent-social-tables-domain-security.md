---
api_specs:
- filename: cvent-social-tables-openapi.json
  format: json
  label: Social Tables Events API (Legacy)
  slug: events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cvent-social-tables/refs/heads/main/openapi/cvent-social-tables-openapi.json
description: ''
domains:
- caa:
  - 0 issue "digicert.com"
  - 0 issue "letsencrypt.org"
  - 0 issuewild "amazon.com"
  - 0 issuewild "digicert.com"
  - 0 issue "amazon.com"
  - 0 issue "comodo.com"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: socialtables.com
  spf: true
hosts:
- cert_expires: Mar  4 23:59:59 2027 GMT
  host: www.socialtables.com
  hsts: true
  hsts_max_age: 86400
  https: true
  tls_version: TLSv1.2
- cert_expires: Sep 18 23:59:59 2026 GMT
  host: developer.socialtables.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 28 23:59:59 2026 GMT
  host: api.socialtables.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Cvent Social Tables Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Cvent Social Tables, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.2); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Cvent Social Tables
provider_slug: cvent-social-tables
slug: cvent-social-tables-domain-security
source_filename: cvent-social-tables-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.socialtables.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Mar  4 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 86400\n- host: developer.socialtables.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 18 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.socialtables.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Oct 28 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: socialtables.com\n  dnssec: false\n  caa:\n  - 0 issue \"digicert.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issuewild \"amazon.com\"\n  - 0 issuewild \"digicert.com\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"comodo.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cvent-social-tables/refs/heads/main/security/cvent-social-tables-domain-security.yml
summary_line: TLSv1.2 · HSTS · DMARC
tags:
- 3D Design
- Catering
- Diagramming
- Event Design
- Event Management
- Events
- Floor Plans
- Hospitality
- Hotel
- Meetings
- Seating
- Seating Charts
- Venues
---
