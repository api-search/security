---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: listofbooks.net
  spf: true
hosts:
- cert_expires: Dec 22 08:11:37 2026 GMT
  host: www.listofbooks.net
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: List Of Books Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for List Of Books, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: List Of Books
provider_slug: listofbooks-net
slug: listofbooks-net-domain-security
source_filename: listofbooks-net-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-16'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.listofbooks.net\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 22 08:11:37 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: listofbooks.net\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/listofbooks-net/security/listofbooks-net-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Book
- Catalog
- Open Data
- Literature
- Free
---
