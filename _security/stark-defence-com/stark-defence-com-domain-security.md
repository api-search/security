---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: stark-defence.com
  spf: true
hosts:
- cert_expires: Jan 14 10:52:28 2027 GMT
  host: stark-defence.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Stark Defence Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for STARK, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: STARK
provider_slug: stark-defence-com
slug: stark-defence-com-domain-security
source_filename: stark-defence-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-23'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: stark-defence.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 14 10:52:28 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: stark-defence.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/stark-defence-com/security/stark-defence-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Defence
- Autonomous
- Unmanned Systems
- Weaponry Integration
- Government
- Commercial
---
