---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: oxforddictionaries.com
  spf: true
hosts:
- cert_expires: Sep 20 08:09:22 2026 GMT
  host: developer.oxforddictionaries.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Oxford Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Oxford, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Oxford
provider_slug: oxford
slug: oxford-domain-security
source_filename: oxford-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: developer.oxforddictionaries.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Sep 20 08:09:22 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: oxforddictionaries.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/oxford/refs/heads/main/security/oxford-domain-security.yml
summary_line: TLSv1.2 · HSTS · DMARC
tags:
- Dictionaries
- Public APIs
---
