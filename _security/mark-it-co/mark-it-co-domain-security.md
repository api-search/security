---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: mark-it.co
  spf: true
hosts:
- cert_expires: Jan  1 22:45:11 2027 GMT
  host: mark-it.co
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: MarkIt Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for MarkIt, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: MarkIt
provider_slug: mark-it-co
slug: mark-it-co-domain-security
source_filename: mark-it-co-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: mark-it.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  1 22:45:11 2027 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: mark-it.co\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/mark-it-co/security/mark-it-co-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Artificial Intelligence
- Bookmarking
- Content Organization
- Semantic Search
- Privacy
---
