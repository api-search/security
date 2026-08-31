---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: techsee.com
  spf: false
hosts:
- cert_expires: Nov  2 18:43:37 2026 GMT
  host: techsee.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Techsee Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for TechSee, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: TechSee
provider_slug: techsee
slug: techsee-domain-security
source_filename: techsee-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-29'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: techsee.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  2 18:43:37 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: techsee.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/techsee/refs/heads/main/security/techsee-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Visual Assistance
- Customer Experience
- Customer Service
- Contact Center
- Computer Vision
- Augmented Reality
- Artificial Intelligence
- Field Service
- Remote Support
- Video
- Telecommunications
---
