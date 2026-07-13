---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: dragoneye.ai
  spf: true
hosts:
- cert_expires: Sep 13 14:27:49 2026 GMT
  host: dragoneye.ai
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  2 04:00:17 2026 GMT
  host: docs.dragoneye.ai
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Dragoneye Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Dragoneye, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Dragoneye
provider_slug: dragoneye
slug: dragoneye-domain-security
source_filename: dragoneye-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: dragoneye.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 13 14:27:49 2026 GMT\n  hsts: false\n- host: docs.dragoneye.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  2 04:00:17 2026 GMT\n  hsts: false\ndomains:\n- domain: dragoneye.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/dragoneye/refs/heads/main/security/dragoneye-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Artificial Intelligence
- Computer Vision
- Image Recognition
- Video Recognition
- Machine Learning
---
