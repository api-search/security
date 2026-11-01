---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: sparkgeo.com
  spf: true
hosts:
- cert_expires: Jan  8 01:08:35 2027 GMT
  host: sparkgeo.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Sparkgeo Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Sparkgeo, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Sparkgeo
provider_slug: sparkgeo
slug: sparkgeo-domain-security
source_filename: sparkgeo-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-23'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: sparkgeo.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  8 01:08:35 2027 GMT\n  hsts: false\ndomains:\n- domain: sparkgeo.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/sparkgeo/security/sparkgeo-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Geospatial Software Development
- Location-based Analytics
- Data Engineering
- Operational Intelligence
- Managed Geospatial Services
- Cloud-native Platforms
---
