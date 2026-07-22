---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: greeneye.ag
  spf: true
hosts:
- cert_expires: Sep 26 12:50:45 2026 GMT
  host: greeneye.ag
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Green Eye Technology Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Green Eye Technology, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Green Eye Technology
provider_slug: green-eye-technology
slug: green-eye-technology-domain-security
source_filename: green-eye-technology-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: greeneye.ag\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 26 12:50:45 2026 GMT\n  hsts: false\ndomains:\n- domain: greeneye.ag\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/green-eye-technology/refs/heads/main/security/green-eye-technology-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Agriculture
- AgTech
- Precision Agriculture
- Artificial Intelligence
- Computer Vision
- Weed Management
- Precision Spraying
---
