---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: klodkot.ai
  spf: false
hosts:
- cert_expires: Feb  8 10:15:18 2027 GMT
  host: klodkot.ai
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Клод Кот Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Клод Кот, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Клод Кот
provider_slug: klodkot-ai
slug: klodkot-ai-domain-security
source_filename: klodkot-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-13'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: klodkot.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  8 10:15:18 2027 GMT\n  hsts: false\ndomains:\n- domain: klodkot.ai\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/klodkot-ai/security/klodkot-ai-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
---
