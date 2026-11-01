---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: orshot.com
  spf: true
hosts:
- cert_expires: Jan 23 19:04:28 2027 GMT
  host: orshot.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Orshot Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for orshot-com, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: orshot-com
provider_slug: orshot-com
slug: orshot-com-domain-security
source_filename: orshot-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: orshot.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 23 19:04:28 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: orshot.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/orshot-com/security/orshot-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- API
- Media
- Automation
- AI
---
