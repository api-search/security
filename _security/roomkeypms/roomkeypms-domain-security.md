---
api_specs:
- filename: roomkeypms-openapi.yml
  format: yaml
  label: RoomKeyPMS Reservation Data API
  slug: roomkeypms-reservation-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/roomkeypms/refs/heads/main/openapi/roomkeypms-openapi.yml
- filename: roomkeypms-openapi.yml
  format: yaml
  label: RoomKeyPMS POS Integration API
  slug: roomkeypms-pos-integration-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/roomkeypms/refs/heads/main/openapi/roomkeypms-openapi.yml
- filename: roomkeypms-openapi.yml
  format: yaml
  label: RoomKeyPMS Statistics and Forecasts API
  slug: roomkeypms-statistics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/roomkeypms/refs/heads/main/openapi/roomkeypms-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: roomkeypms.com
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: welcometorsi.net
  spf: false
hosts:
- cert_expires: Aug 30 16:22:01 2026 GMT
  host: roomkeypms.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  9 10:57:48 2026 GMT
  host: support.roomkeypms.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 18 03:01:32 2026 GMT
  host: www.welcometorsi.net
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Roomkeypms Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for RoomKeyPMS, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: RoomKeyPMS
provider_slug: roomkeypms
slug: roomkeypms-domain-security
source_filename: roomkeypms-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: roomkeypms.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 30 16:22:01 2026 GMT\n  hsts: false\n- host: support.roomkeypms.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  9 10:57:48 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: www.welcometorsi.net\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 18 03:01:32 2026 GMT\n  hsts: false\ndomains:\n- domain: roomkeypms.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: welcometorsi.net\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/roomkeypms/refs/heads/main/security/roomkeypms-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Hospitality
- Hotel Technology
- Property Management System
- PMS
- Reservations
- POS
- Gated API
---
