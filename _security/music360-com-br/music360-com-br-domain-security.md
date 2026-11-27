---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: music360.com.br
  spf: true
hosts:
- cert_expires: Dec 20 10:19:32 2026 GMT
  host: music360.com.br
  hsts: true
  hsts_max_age: 0
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Music360 Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Music360, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Music360
provider_slug: music360-com-br
slug: music360-com-br-domain-security
source_filename: music360-com-br-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: music360.com.br\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 20 10:19:32 2026 GMT\n  hsts: true\n  hsts_max_age: 0\ndomains:\n- domain: music360.com.br\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/music360-com-br/security/music360-com-br-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Music
- Software-as-a-Service
- Entertainment
- Brazil
---
