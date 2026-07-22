---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: neurala.com
  spf: true
hosts:
- cert_expires: Oct  5 13:36:25 2026 GMT
  host: neurala.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Neurala Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Neurala, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Neurala
provider_slug: neurala
slug: neurala-domain-security
source_filename: neurala-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: neurala.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  5 13:36:25 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: neurala.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/neurala/refs/heads/main/security/neurala-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Artificial Intelligence
- Computer Vision
- Machine Learning
- Edge AI
- Deep Learning
- Visual Inspection
- Manufacturing
---
