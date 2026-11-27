---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: prismm.com
  spf: true
hosts:
- cert_expires: Jan  1 08:12:49 2027 GMT
  host: prismm.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Prismm Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Prismm, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Prismm
provider_slug: prismm
slug: prismm-domain-security
source_filename: prismm-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-16'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: prismm.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  1 08:12:49 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: prismm.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/prismm/security/prismm-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Spatial Design
- 3D Visualization
- Event Planning
- Venue Marketing
- Collaboration
---
