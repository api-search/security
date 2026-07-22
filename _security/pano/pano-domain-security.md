---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: pano.ai
  spf: true
hosts:
- cert_expires: Oct 15 16:12:24 2026 GMT
  host: pano.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Pano Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Pano, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Pano
provider_slug: pano
slug: pano-domain-security
source_filename: pano-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: pano.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 15 16:12:24 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: pano.ai\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/pano/refs/heads/main/security/pano-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Wildfire Detection
- Fire Detection
- Situational Awareness
- Geospatial
- Computer Vision
- Artificial Intelligence
- Emergency Management
- Public Safety
---
