---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: openfreemap.org
  spf: true
hosts:
- cert_expires: Jan  5 06:14:03 2027 GMT
  host: openfreemap.org
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Openfreemap Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for OpenFreeMap vector styles, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: OpenFreeMap vector styles
provider_slug: openfreemap
slug: openfreemap-domain-security
source_filename: openfreemap-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-28'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: openfreemap.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  5 06:14:03 2027 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: openfreemap.org\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/openfreemap/security/openfreemap-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Open-source
- Mapping
- GIS
- Vector Tiles
- Free Hosting
---
