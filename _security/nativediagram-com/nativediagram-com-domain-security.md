---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: nativediagram.com
  spf: true
hosts:
- cert_expires: Feb 15 04:56:53 2027 GMT
  host: nativediagram.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: NativeDiagram Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for NativeDiagram, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: NativeDiagram
provider_slug: nativediagram-com
slug: nativediagram-com-domain-security
source_filename: nativediagram-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: nativediagram.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 15 04:56:53 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: nativediagram.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/nativediagram-com/security/nativediagram-com-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- SmartArt
- AI Assistant
- Microsoft Office
---
