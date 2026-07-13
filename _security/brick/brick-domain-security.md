---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: brickschema.org
  spf: true
hosts:
- cert_expires: Sep 23 22:05:51 2026 GMT
  host: brickschema.org
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Brick Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for BRICK Schema, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: BRICK Schema
provider_slug: brick
slug: brick-domain-security
source_filename: brick-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: brickschema.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 23 22:05:51 2026 GMT\n  hsts: false\ndomains:\n- domain: brickschema.org\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/brick/refs/heads/main/security/brick-domain-security.yml
summary_line: TLSv1.3
tags:
- Building Information Modeling
- BIM
- Smart Buildings
- Ontology
- Semantic Web
- IoT
- HVAC
- Energy Management
---
