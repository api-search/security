---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: maplibre.org
  spf: false
hosts:
- cert_expires: Jan 26 12:18:25 2027 GMT
  host: maplibre.org
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: MapLibre Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for MapLibre, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: MapLibre
provider_slug: maplibre
slug: maplibre-domain-security
source_filename: maplibre-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-16'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: maplibre.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 26 12:18:25 2027 GMT\n  hsts: false\ndomains:\n- domain: maplibre.org\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/maplibre/security/maplibre-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- Mapping
- Open Source
- Geospatial
- JavaScript
---
