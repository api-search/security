---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: promptattack.com
  spf: false
hosts:
- cert_expires: Dec 19 21:12:28 2026 GMT
  host: promptattack.com
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Promptattack Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Prompt Attack, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Prompt Attack
provider_slug: promptattack
slug: promptattack-domain-security
source_filename: promptattack-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: promptattack.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 19 21:12:28 2026 GMT\n  hsts: null\ndomains:\n- domain: promptattack.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/promptattack/security/promptattack-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
---
