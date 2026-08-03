---
api_specs:
- filename: inrix-user-accounts-openapi-original.json
  format: json
  label: INRIX User Accounts System (UAS) API
  slug: inrix-user-accounts-system-uas-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/inrix/refs/heads/main/openapi/inrix-user-accounts-openapi-original.json
- filename: inrix-parkme-openapi-original.json
  format: json
  label: INRIX Parking API (INRIX Parking Services 3.0 / ParkMe)
  slug: inrix-parking-api-inrix-parking-services-30-parkme
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/inrix/refs/heads/main/openapi/inrix-parkme-openapi-original.json
- filename: inrix-signals-analytics-openapi-original.json
  format: json
  label: INRIX Signals Analytics API
  slug: inrix-signals-analytics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/inrix/refs/heads/main/openapi/inrix-signals-analytics-openapi-original.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: inrix.com
  spf: true
hosts:
- cert_expires: Oct 12 11:10:55 2026 GMT
  host: inrix.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan  2 23:59:59 2027 GMT
  host: docs.inrix.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 21 23:59:59 2026 GMT
  host: uas-api.inrix.com
  hsts: false
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Inrix Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for INRIX, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: INRIX
provider_slug: inrix
slug: inrix-domain-security
source_filename: inrix-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-01'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: inrix.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 12 11:10:55 2026 GMT\n  hsts: null\n- host: docs.inrix.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  2 23:59:59 2027 GMT\n  hsts: false\n- host: uas-api.inrix.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Nov 21 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: inrix.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/inrix/refs/heads/main/security/inrix-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Transportation
- Traffic
- Mobility
- Parking
- Geospatial
- Location Data
- Analytics
- Automotive
- Smart Cities
- Routing
- Connected Vehicles
- Road Network
- Data
- Fleet
- Intelligent Transportation Systems
---
