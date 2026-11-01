---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: promptoctopus.com
  spf: false
hosts:
- cert_expires: Jan 14 10:07:18 2027 GMT
  host: promptoctopus.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Promptoctopus Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Prompt Octopus, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Prompt Octopus
provider_slug: promptoctopus
slug: promptoctopus-domain-security
source_filename: promptoctopus-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: promptoctopus.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 14 10:07:18 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: promptoctopus.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/promptoctopus/security/promptoctopus-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Artificial Intelligence
- Prompt Engineering
- Developer Tools
- LLM Evaluation
---
