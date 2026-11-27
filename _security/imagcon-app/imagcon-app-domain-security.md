---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: imagcon.app
  spf: true
hosts:
- cert_expires: Jan 18 22:56:52 2027 GMT
  host: imagcon.app
  hsts: true
  hsts_max_age: 31556926
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Imagcon Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Imagcon, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Imagcon
provider_slug: imagcon-app
slug: imagcon-app-domain-security
source_filename: imagcon-app-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-12'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: imagcon.app\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 18 22:56:52 2027 GMT\n  hsts: true\n  hsts_max_age: 31556926\ndomains:\n- domain: imagcon.app\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/imagcon-app/security/imagcon-app-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Artificial Intelligence
- Icon
- Generator
- Developer Tools
- Imagcon
---
