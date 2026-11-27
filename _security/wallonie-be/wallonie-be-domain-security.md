---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: wallonie.be
  spf: true
hosts:
- cert_expires: Jan  2 01:50:28 2027 GMT
  host: geoportail.wallonie.be
  hsts: true
  hsts_max_age: 15724800
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Géoportail de la Wallonie Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Géoportail de la Wallonie, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Géoportail de la Wallonie
provider_slug: wallonie-be
slug: wallonie-be-domain-security
source_filename: wallonie-be-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-10'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: geoportail.wallonie.be\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  2 01:50:28 2027 GMT\n  hsts: true\n  hsts_max_age: 15724800\ndomains:\n- domain: wallonie.be\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/wallonie-be/security/wallonie-be-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Government
- Geospatial
- OGC
- INSPIRE
- Open Data
- Belgium
- Maps
---
