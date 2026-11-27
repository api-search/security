---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: zoomeye.ai
  spf: true
hosts:
- cert_expires: Jan 17 23:59:59 2027 GMT
  host: www.zoomeye.ai
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: ZoomEye Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for ZoomEye, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: ZoomEye
provider_slug: zoomeye
slug: zoomeye-domain-security
source_filename: zoomeye-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-16'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.zoomeye.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 17 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: zoomeye.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/zoomeye/security/zoomeye-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Cybersecurity
- Search Engines
- Asset Discovery
---
