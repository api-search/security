---
api_specs:
- filename: ezee-openapi.yml
  format: yaml
  label: eZee Reservations & Bookings API
  slug: ezee-reservations-bookings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ezee/refs/heads/main/openapi/ezee-openapi.yml
- filename: ezee-openapi.yml
  format: yaml
  label: eZee Room Inventory & Rates API
  slug: ezee-room-inventory-rates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ezee/refs/heads/main/openapi/ezee-openapi.yml
- filename: ezee-openapi.yml
  format: yaml
  label: eZee Guests & Configuration API
  slug: ezee-guests-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ezee/refs/heads/main/openapi/ezee-openapi.yml
- filename: ezee-openapi.yml
  format: yaml
  label: eZee Centrix Channel Manager API
  slug: ezee-channel-manager-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ezee/refs/heads/main/openapi/ezee-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: ezeetechnosys.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: ipms247.com
  spf: false
hosts:
- cert_expires: Oct  5 02:29:59 2026 GMT
  host: www.ezeetechnosys.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  3 13:42:03 2026 GMT
  host: api.ezeetechnosys.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  2 23:59:59 2026 GMT
  host: live.ipms247.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Ezee Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for eZee Technosys, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: eZee Technosys
provider_slug: ezee
slug: ezee-domain-security
source_filename: ezee-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.ezeetechnosys.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  5 02:29:59 2026 GMT\n  hsts: false\n- host: api.ezeetechnosys.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  3 13:42:03 2026 GMT\n  hsts: false\n- host: live.ipms247.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  2 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: ezeetechnosys.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: ipms247.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ezee/refs/heads/main/security/ezee-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Hospitality
- Hotel
- PMS
- Channel Manager
- Reservations
---
