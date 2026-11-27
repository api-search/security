---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: mondovo.com
  spf: true
hosts:
- cert_expires: Feb  5 12:38:23 2027 GMT
  host: mondovo.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Mondovo Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Mondovo, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Mondovo
provider_slug: mondovo-com
slug: mondovo-com-domain-security
source_filename: mondovo-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: mondovo.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  5 12:38:23 2027 GMT\n  hsts: false\ndomains:\n- domain: mondovo.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/mondovo-com/security/mondovo-com-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Artificial Intelligence
- Website Builder
- Marketing Automation
- Small Business
- Agency
---
