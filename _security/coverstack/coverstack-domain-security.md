---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: coverstack.in
  spf: true
hosts:
- cert_expires: Nov 18 07:42:17 2026 GMT
  host: coverstack.in
  hsts: false
  https: true
  tls_version: TLSv1.2
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Coverstack Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for CoverStack, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: CoverStack
provider_slug: coverstack
slug: coverstack-domain-security
source_filename: coverstack-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: coverstack.in\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Nov 18 07:42:17 2026 GMT\n  hsts: false\ndomains:\n- domain: coverstack.in\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/coverstack/security/coverstack-domain-security.yml
summary_line: TLSv1.2 · DMARC
tags:
- No-Code
- API Platform
- Data Integration
- Automation
- Software-as-a-Service
---
