---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: dropthehassle.com
  spf: true
hosts:
- cert_expires: Jan 30 09:22:08 2027 GMT
  host: dropthehassle.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: DropTheHassle Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for DropTheHassle, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: DropTheHassle
provider_slug: dropthehassle-com
slug: dropthehassle-com-domain-security
source_filename: dropthehassle-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-06'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: dropthehassle.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 30 09:22:08 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: dropthehassle.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/dropthehassle-com/security/dropthehassle-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Hosting
- Artificial Intelligence
- Domain
- Email
- Free
- Developers
---
