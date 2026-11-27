---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dns_aid:
    checked: '2026-11-25'
    published: false
  dnssec: false
  domain: tableall.com
  spf: true
hosts:
- cert_expires: Feb  2 23:59:59 2027 GMT
  host: tableall.com
  hsts: false
  https: true
  tls_version: TLSv1.2
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: TableAll Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for TableAll, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: TableAll
provider_slug: tableall-com
slug: tableall-com-domain-security
source_filename: tableall-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-25'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: tableall.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Feb  2 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: tableall.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n  dns_aid:\n    checked: '2026-11-25'\n    published: false\n"
source_yaml_url: https://artifacts.apis.io/tableall-com/security/tableall-com-domain-security.yml
summary_line: TLSv1.2 · DMARC
tags:
- Restaurant
- Reservation
- Japan
- API
- Travel
---
