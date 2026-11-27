---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: hlist.cc
  spf: true
hosts:
- cert_expires: Jan  5 07:30:18 2027 GMT
  host: hlist.cc
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: HList Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for HList, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: HList
provider_slug: hlist-cc
slug: hlist-cc-domain-security
source_filename: hlist-cc-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: hlist.cc\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  5 07:30:18 2027 GMT\n  hsts: false\ndomains:\n- domain: hlist.cc\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/hlist-cc/security/hlist-cc-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Artificial Intelligence
- Directory
- Tools
- Open Data
---
