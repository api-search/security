---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: flowboxx.de
  spf: true
hosts:
- cert_expires: Feb  1 10:15:43 2027 GMT
  host: flowboxx.de
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: flowboxx Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for flowboxx, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: flowboxx
provider_slug: flowboxx-de
slug: flowboxx-de-domain-security
source_filename: flowboxx-de-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-08'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: flowboxx.de\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  1 10:15:43 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: flowboxx.de\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/flowboxx-de/security/flowboxx-de-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Web Development
- SEO
- AI Integration
- German Market
- Small Business
---
