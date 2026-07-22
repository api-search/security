---
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issue ";"
  - 0 issue "amazonaws.com"
  - 0 iodef "mailto:security@doxel.ai"
  - 0 issue "pki.goog"
  - 0 issue "awstrust.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: doxel.ai
  spf: true
hosts:
- cert_expires: Aug 17 08:57:03 2026 GMT
  host: www.doxel.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Doxel Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Doxel, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Doxel
provider_slug: doxel
slug: doxel-domain-security
source_filename: doxel-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.doxel.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 17 08:57:03 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: doxel.ai\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \";\"\n  - 0 issue \"amazonaws.com\"\n  - 0 iodef \"mailto:security@doxel.ai\"\n  - 0 issue \"pki.goog\"\n  - 0 issue \"awstrust.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/doxel/refs/heads/main/security/doxel-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Construction
- Construction Technology
- ConTech
- AI
- Computer Vision
- Reality Capture
- Progress Tracking
- BIM
- Building Information Modeling
- Earned Value
- Schedule Management
- Budget Tracking
- Capital Projects
- Data Centers
- Healthcare Construction
- Industrial Construction
- Drones
- 360 Cameras
---
