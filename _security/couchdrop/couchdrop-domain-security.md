---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: couchdrop.io
  spf: true
hosts:
- cert_expires: Apr 15 23:59:59 2027 GMT
  host: couchdrop.io
  hsts: true
  hsts_max_age: 3628800
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Couchdrop Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Couchdrop, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Couchdrop
provider_slug: couchdrop
slug: couchdrop-domain-security
source_filename: couchdrop-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: couchdrop.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Apr 15 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 3628800\ndomains:\n- domain: couchdrop.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/couchdrop/security/couchdrop-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- File Transfer
- SFTP
- Automation
- Integration
- Cloud
---
