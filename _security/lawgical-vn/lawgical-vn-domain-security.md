---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: lawgical.vn
  spf: true
hosts:
- cert_expires: Dec 25 01:43:52 2026 GMT
  host: lawgical.vn
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Lawgical Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Lawgical, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Lawgical
provider_slug: lawgical-vn
slug: lawgical-vn-domain-security
source_filename: lawgical-vn-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-14'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: lawgical.vn\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 25 01:43:52 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: lawgical.vn\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/lawgical-vn/security/lawgical-vn-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Law
- Artificial Intelligence
- Legal Tech
- Vietnam
---
