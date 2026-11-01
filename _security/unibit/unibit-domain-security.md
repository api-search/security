---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: unibit.ai
  spf: true
hosts:
- cert_expires: Dec 25 00:28:03 2026 GMT
  host: unibit.ai
  hsts: true
  hsts_max_age: 31556926
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Unibit Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for UniBit, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: UniBit
provider_slug: unibit
slug: unibit-domain-security
source_filename: unibit-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: unibit.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 25 00:28:03 2026 GMT\n  hsts: true\n  hsts_max_age: 31556926\ndomains:\n- domain: unibit.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/unibit/security/unibit-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- IoT
- Device Management
- API Platform
- Cloud Services
- Analytics
---
