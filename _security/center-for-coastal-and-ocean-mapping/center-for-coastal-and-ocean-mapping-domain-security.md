---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: unh.edu
  spf: true
hosts:
- cert_expires: Nov 15 23:59:59 2026 GMT
  host: ccom.unh.edu
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Center For Coastal And Ocean Mapping Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Center for Coastal and Ocean Mapping, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Center for Coastal and Ocean Mapping
provider_slug: center-for-coastal-and-ocean-mapping
slug: center-for-coastal-and-ocean-mapping-domain-security
source_filename: center-for-coastal-and-ocean-mapping-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-23'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: ccom.unh.edu\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 15 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: unh.edu\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/center-for-coastal-and-ocean-mapping/security/center-for-coastal-and-ocean-mapping-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Research
- OceanMapping
- Geospatial
- OpenData
---
