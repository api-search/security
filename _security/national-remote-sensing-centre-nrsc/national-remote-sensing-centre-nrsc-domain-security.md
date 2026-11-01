---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: nrsc.gov.in
  spf: true
hosts:
- cert_expires: Dec 21 14:12:15 2026 GMT
  host: www.nrsc.gov.in
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: National Remote Sensing Centre Nrsc Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for National Remote Sensing Centre (NRSC), probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: National Remote Sensing Centre (NRSC)
provider_slug: national-remote-sensing-centre-nrsc
slug: national-remote-sensing-centre-nrsc-domain-security
source_filename: national-remote-sensing-centre-nrsc-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-26'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.nrsc.gov.in\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 21 14:12:15 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: nrsc.gov.in\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/national-remote-sensing-centre-nrsc/security/national-remote-sensing-centre-nrsc-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Remote Sensing
- Geospatial Data
- Satellite Services
- Disaster Management
- Agriculture
- Land Use
- Water Resources
- Urban Planning
---
