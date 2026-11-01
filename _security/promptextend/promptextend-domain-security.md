---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: promptextend.com
  spf: false
hosts:
- cert_expires: Dec 19 15:48:25 2026 GMT
  host: promptextend.com
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Promptextend Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for PromptExtend, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: PromptExtend
provider_slug: promptextend
slug: promptextend-domain-security
source_filename: promptextend-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: promptextend.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 19 15:48:25 2026 GMT\n  hsts: null\ndomains:\n- domain: promptextend.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/promptextend/security/promptextend-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
---
