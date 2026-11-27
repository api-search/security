---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: buildcheap.app
  spf: false
hosts:
- cert_expires: Jan  4 16:18:23 2027 GMT
  host: buildcheap.app
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: BuildCheap Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for BuildCheap, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: BuildCheap
provider_slug: buildcheap-app
slug: buildcheap-app-domain-security
source_filename: buildcheap-app-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-03'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: buildcheap.app\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  4 16:18:23 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: buildcheap.app\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/buildcheap-app/security/buildcheap-app-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Artificial Intelligence
- No-Code
- Platform
- Software-as-a-Service
- Automation
---
