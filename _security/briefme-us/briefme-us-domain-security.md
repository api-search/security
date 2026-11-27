---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: briefme.us
  spf: true
hosts:
- cert_expires: Jan  6 13:57:19 2027 GMT
  host: briefme.us
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: BriefMe Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for BriefMe, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: BriefMe
provider_slug: briefme-us
slug: briefme-us-domain-security
source_filename: briefme-us-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-03'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: briefme.us\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  6 13:57:19 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: briefme.us\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/briefme-us/security/briefme-us-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Timer
- Meetings
- Productivity
- Software-as-a-Service
- Free
---
