---
api_specs:
- filename: index-v1.json
  format: json
  label: Geofabrik Download API
  slug: download-api
  spec_type: OpenAPI
  url: https://download.geofabrik.de/index-v1.json
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: geofabrik.de
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: overpass-api.de
  spf: false
hosts:
- cert_expires: Sep 21 06:45:43 2026 GMT
  host: www.geofabrik.de
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 21 13:14:23 2026 GMT
  host: download.geofabrik.de
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 20 05:53:56 2026 GMT
  host: overpass-api.de
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Geofabrik Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Geofabrik, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Geofabrik
provider_slug: geofabrik
slug: geofabrik-domain-security
source_filename: geofabrik-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.geofabrik.de\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 21 06:45:43 2026 GMT\n  hsts: false\n- host: download.geofabrik.de\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 21 13:14:23 2026 GMT\n  hsts: false\n- host: overpass-api.de\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 20 05:53:56 2026 GMT\n  hsts: false\ndomains:\n- domain: geofabrik.de\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n- domain: overpass-api.de\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/geofabrik/refs/heads/main/security/geofabrik-domain-security.yml
summary_line: TLSv1.3
tags:
- OpenStreetMap
- Geospatial
- GIS
- Maps
- Download
- OSM
- Routing
- Geocoding
---
