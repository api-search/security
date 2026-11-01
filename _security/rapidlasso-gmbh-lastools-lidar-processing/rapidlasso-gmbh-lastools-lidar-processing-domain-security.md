---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: rapidlasso.de
  spf: true
hosts:
- cert_expires: Jan  3 01:48:13 2027 GMT
  host: rapidlasso.de
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Rapidlasso Gmbh Lastools Lidar Processing Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for rapidlasso GmbH - LAStools LiDAR processing, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: rapidlasso GmbH - LAStools LiDAR processing
provider_slug: rapidlasso-gmbh-lastools-lidar-processing
slug: rapidlasso-gmbh-lastools-lidar-processing-domain-security
source_filename: rapidlasso-gmbh-lastools-lidar-processing-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-23'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: rapidlasso.de\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  3 01:48:13 2027 GMT\n  hsts: false\ndomains:\n- domain: rapidlasso.de\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/rapidlasso-gmbh-lastools-lidar-processing/security/rapidlasso-gmbh-lastools-lidar-processing-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- LiDAR
- Geospatial
- PointCloud
- Surveying
---
