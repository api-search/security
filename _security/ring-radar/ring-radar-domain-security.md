---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: ringradar.com
  spf: true
hosts:
- cert_expires: Aug 31 23:07:47 2026 GMT
  host: ringradar.com
  hsts: true
  hsts_max_age: 60
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Ring Radar Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Ring Radar, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Ring Radar
provider_slug: ring-radar
slug: ring-radar-domain-security
source_filename: ring-radar-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: ringradar.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 31 23:07:47 2026 GMT\n  hsts: true\n  hsts_max_age: 60\ndomains:\n- domain: ringradar.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ring-radar/refs/heads/main/security/ring-radar-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Horse Shows
- Equestrian
- Event Management
- Sports
- Software
- SaaS
---
