---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: autocore.ai
  spf: true
hosts:
- cert_expires: Nov  5 08:39:02 2026 GMT
  host: autocore.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Autocore Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Autocore, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Autocore
provider_slug: autocore
slug: autocore-domain-security
source_filename: autocore-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-26'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: autocore.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  5 08:39:02 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: autocore.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/autocore/refs/heads/main/security/autocore-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Automotive
- Robotics
- Software
- Artificial Intelligence
---
