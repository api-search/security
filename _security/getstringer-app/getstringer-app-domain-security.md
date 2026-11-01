---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: getstringer.app
  spf: true
hosts:
- cert_expires: Jan 21 20:04:51 2027 GMT
  host: getstringer.app
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Getstringer App Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for getstringer-app, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: getstringer-app
provider_slug: getstringer-app
slug: getstringer-app-domain-security
source_filename: getstringer-app-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: getstringer.app\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 21 20:04:51 2027 GMT\n  hsts: false\ndomains:\n- domain: getstringer.app\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/getstringer-app/security/getstringer-app-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- Autonomous
- Micropayment
- AI
- Tools
---
