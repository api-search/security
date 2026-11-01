---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: openhistoricalmap.org
  spf: false
hosts:
- cert_expires: Jan  5 03:55:13 2027 GMT
  host: openhistoricalmap.org
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Openhistoricalmap Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for OpenHistoricalMap time-aware basemap style, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: OpenHistoricalMap time-aware basemap style
provider_slug: openhistoricalmap
slug: openhistoricalmap-domain-security
source_filename: openhistoricalmap-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-28'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: openhistoricalmap.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  5 03:55:13 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: openhistoricalmap.org\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/openhistoricalmap/security/openhistoricalmap-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Mapping
- Historical
- Open-Source
- Nonprofit
- Geospatial
- Community
---
