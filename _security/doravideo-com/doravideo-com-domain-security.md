---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: doravideo.com
  spf: true
hosts:
- cert_expires: Jan  2 04:12:05 2027 GMT
  host: doravideo.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Saga Labs Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Saga Labs, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Saga Labs
provider_slug: doravideo-com
slug: doravideo-com-domain-security
source_filename: doravideo-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-05'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: doravideo.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  2 04:12:05 2027 GMT\n  hsts: false\ndomains:\n- domain: doravideo.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/doravideo-com/security/doravideo-com-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Artificial Intelligence
- Video
- Generation
- Platform
- Software-as-a-Service
---
