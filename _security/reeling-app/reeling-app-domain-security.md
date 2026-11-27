---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: reeling.app
  spf: true
hosts:
- cert_expires: Feb  3 16:03:41 2027 GMT
  host: reeling.app
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Reeling Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Reeling, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Reeling
provider_slug: reeling-app
slug: reeling-app-domain-security
source_filename: reeling-app-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-16'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: reeling.app\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  3 16:03:41 2027 GMT\n  hsts: false\ndomains:\n- domain: reeling.app\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/reeling-app/security/reeling-app-domain-security.yml
summary_line: TLSv1.3
tags:
- Video Scheduling
- AI Content Generation
- Multi-Channel Publishing
- Developer Tools
- Creator Tools
---
