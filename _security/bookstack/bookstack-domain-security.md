---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: bookstackapp.com
  spf: true
hosts:
- cert_expires: Sep 23 20:17:47 2026 GMT
  host: www.bookstackapp.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 23 20:17:47 2026 GMT
  host: demo.bookstackapp.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Bookstack Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for BookStack, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: BookStack
provider_slug: bookstack
slug: bookstack-domain-security
source_filename: bookstack-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.bookstackapp.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 23 20:17:47 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: demo.bookstackapp.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 23 20:17:47 2026 GMT\n  hsts: false\ndomains:\n- domain: bookstackapp.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bookstack/refs/heads/main/security/bookstack-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Wiki
- Documentation
- Knowledge Base
- Self-Hosted
- Open Source
- Content Management
---
