---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: orreco.ai
  spf: false
hosts:
- cert_expires: Nov 30 00:40:22 2026 GMT
  host: orreco.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Orrecoai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Orreco.ai, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Orreco.ai
provider_slug: orrecoai
slug: orrecoai-domain-security
source_filename: orrecoai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-24'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: orreco.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 30 00:40:22 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: orreco.ai\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/orrecoai/security/orrecoai-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Sports
- AI
- Analytics
- HealthTech
- Company
---
