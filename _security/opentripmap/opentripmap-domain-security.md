---
api_specs:
- filename: opentripmap-openapi.json
  format: json
  label: OpenTripMap API
  slug: opentripmap-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/opentripmap/refs/heads/main/openapi/opentripmap-openapi.json
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: opentripmap.com
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: opentripmap.org
  spf: true
hosts:
- cert_expires: Sep 27 03:35:14 2026 GMT
  host: opentripmap.com
  hsts: false
  https: true
  tls_version: TLSv1.2
- cert_expires: Aug 18 07:54:39 2026 GMT
  host: dev.opentripmap.org
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 18 13:10:04 2026 GMT
  host: api.opentripmap.com
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Opentripmap Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for OpenTripMap, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: OpenTripMap
provider_slug: opentripmap
slug: opentripmap-domain-security
source_filename: opentripmap-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: opentripmap.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Sep 27 03:35:14 2026 GMT\n  hsts: false\n- host: dev.opentripmap.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 18 07:54:39 2026 GMT\n  hsts: false\n- host: api.opentripmap.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Sep 18 13:10:04 2026 GMT\n  hsts: null\ndomains:\n- domain: opentripmap.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n- domain: opentripmap.org\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/opentripmap/refs/heads/main/security/opentripmap-domain-security.yml
summary_line: TLSv1.2
tags:
- Travel
- Points of Interest
- POI
- Tourism
- Maps
- Geospatial
- OpenStreetMap
- Wikipedia
- Attractions
- Restaurants
- Hotels
- Museums
- REST API
---
