---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: mainroom.ai
  spf: true
hosts:
- cert_expires: Feb  4 23:02:28 2027 GMT
  host: mainroom.ai
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Mainroom Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Mainroom, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Mainroom
provider_slug: mainroom-ai
slug: mainroom-ai-domain-security
source_filename: mainroom-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: mainroom.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  4 23:02:28 2027 GMT\n  hsts: false\ndomains:\n- domain: mainroom.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/mainroom-ai/security/mainroom-ai-domain-security.yml
summary_line: TLSv1.3
tags:
- Artificial Intelligence
- Meetings
- Collaboration
- Productivity
- Video Conferencing
---
