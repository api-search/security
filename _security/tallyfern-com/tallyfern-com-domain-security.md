---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dns_aid:
    checked: '2026-11-26'
    published: false
  dnssec: false
  domain: tallyfern.com
  spf: true
hosts:
- cert_expires: Feb 23 19:50:03 2027 GMT
  host: tallyfern.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Tallyfern Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Tallyfern, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Tallyfern
provider_slug: tallyfern-com
slug: tallyfern-com-domain-security
source_filename: tallyfern-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-26'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: tallyfern.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 23 19:50:03 2027 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: tallyfern.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n  dns_aid:\n    checked: '2026-11-26'\n    published: false\n"
source_yaml_url: https://artifacts.apis.io/tallyfern-com/security/tallyfern-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Templates
- Bookkeeping
- Travel
- Canadian
- AI-assistants
---
