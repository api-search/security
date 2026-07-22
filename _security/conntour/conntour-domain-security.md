---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: conntour.com
  spf: false
hosts:
- cert_expires: Jan  6 23:59:59 2027 GMT
  host: www.conntour.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Conntour Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Conntour, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=none).'
provider_name: Conntour
provider_slug: conntour
slug: conntour-domain-security
source_filename: conntour-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.conntour.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  6 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: conntour.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/conntour/refs/heads/main/security/conntour-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Video Intelligence
- Computer Vision
- Physical Security
- Surveillance
- Artificial Intelligence
- Video Analytics
- Public Safety
---
