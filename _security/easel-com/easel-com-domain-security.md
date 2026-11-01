---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: easel.com
  spf: true
hosts:
- cert_expires: Jan 30 23:59:59 2027 GMT
  host: easel.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Easel Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Easel, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Easel
provider_slug: easel-com
slug: easel-com-domain-security
source_filename: easel-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-29'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: easel.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 30 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: easel.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/easel-com/security/easel-com-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- CNC
- Manufacturing
- Design
- Software
- Maker
- API
---
