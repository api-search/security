---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: send16.com
  spf: true
hosts:
- cert_expires: Jan  1 09:13:59 2027 GMT
  host: send16.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Send16 Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for send16-com, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: send16-com
provider_slug: send16-com
slug: send16-com-domain-security
source_filename: send16-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-31'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: send16.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  1 09:13:59 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: send16.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/send16-com/security/send16-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Email
- Marketing
- Automation
- AI
- SaaS
---
