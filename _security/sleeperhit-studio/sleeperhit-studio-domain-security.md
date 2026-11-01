---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: sleeperhit.studio
  spf: true
hosts:
- cert_expires: Dec  5 05:48:17 2026 GMT
  host: sleeperhit.studio
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Sleeperhit Studio Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for sleeperhit-studio, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: sleeperhit-studio
provider_slug: sleeperhit-studio
slug: sleeperhit-studio-domain-security
source_filename: sleeperhit-studio-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: sleeperhit.studio\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  5 05:48:17 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: sleeperhit.studio\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/sleeperhit-studio/security/sleeperhit-studio-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Audio
- Video
- Podcast
- Enterprise
- Automation
---
