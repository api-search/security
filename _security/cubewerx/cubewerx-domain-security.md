---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: cubewerx.com
  spf: true
hosts:
- cert_expires: Jan 16 17:43:21 2027 GMT
  host: www.cubewerx.com
  hsts: false
  https: true
  tls_version: TLSv1.2
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Cubewerx Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for CubeWerx, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: CubeWerx
provider_slug: cubewerx
slug: cubewerx-domain-security
source_filename: cubewerx-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-23'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.cubewerx.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Jan 16 17:43:21 2027 GMT\n  hsts: false\ndomains:\n- domain: cubewerx.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/cubewerx/security/cubewerx-domain-security.yml
summary_line: TLSv1.2
tags:
- Geospatial
- Data Management
- Web Mapping
- Access Control
- Analytics
- Managed Services
- Cloud
- On-Premise
---
