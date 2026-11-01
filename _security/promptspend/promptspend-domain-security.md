---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: promptspend.com
  spf: true
hosts:
- cert_expires: Dec 30 00:38:38 2026 GMT
  host: promptspend.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Promptspend Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for PromptSpend, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: PromptSpend
provider_slug: promptspend
slug: promptspend-domain-security
source_filename: promptspend-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: promptspend.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 30 00:38:38 2026 GMT\n  hsts: false\ndomains:\n- domain: promptspend.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/promptspend/security/promptspend-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- LLM
- Cost Calculator
- Artificial Intelligence
- Software-as-a-Service
---
