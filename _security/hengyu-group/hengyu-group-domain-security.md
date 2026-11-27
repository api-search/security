---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: hengyu.group
  spf: false
hosts:
- cert_expires: Jan 29 22:07:14 2027 GMT
  host: hengyu.group
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Hengyu Technology Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Hengyu Technology, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Hengyu Technology
provider_slug: hengyu-group
slug: hengyu-group-domain-security
source_filename: hengyu-group-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: hengyu.group\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 29 22:07:14 2027 GMT\n  hsts: false\ndomains:\n- domain: hengyu.group\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/hengyu-group/security/hengyu-group-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
---
