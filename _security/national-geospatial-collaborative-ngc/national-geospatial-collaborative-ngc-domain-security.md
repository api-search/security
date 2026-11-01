---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: nationalgeospatialcollaborative.org
  spf: true
hosts:
- cert_expires: Nov 21 13:16:57 2026 GMT
  host: nationalgeospatialcollaborative.org
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: National Geospatial Collaborative Ngc Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for National Geospatial Collaborative (NGC), probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: National Geospatial Collaborative (NGC)
provider_slug: national-geospatial-collaborative-ngc
slug: national-geospatial-collaborative-ngc-domain-security
source_filename: national-geospatial-collaborative-ngc-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-23'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: nationalgeospatialcollaborative.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 21 13:16:57 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: nationalgeospatialcollaborative.org\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/national-geospatial-collaborative-ngc/security/national-geospatial-collaborative-ngc-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Geospatial
- Nonprofit
- DataSharing
- Collaboration
- OpenSource
---
