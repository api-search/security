---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: ruby.com
  spf: true
hosts:
- cert_expires: Jan 26 06:02:45 2027 GMT
  host: ruby.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Ruby Receptionists Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Ruby Receptionists, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Ruby Receptionists
provider_slug: ruby-receptionists
slug: ruby-receptionists-domain-security
source_filename: ruby-receptionists-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-28'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: ruby.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 26 06:02:45 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: ruby.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/ruby-receptionists/security/ruby-receptionists-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- virtual-receptionist
- live-chat
- 24-7-support
- small-business
- call-answering
---
