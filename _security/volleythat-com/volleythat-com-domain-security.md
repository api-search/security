---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: volleythat.com
  spf: true
hosts:
- cert_expires: Dec 28 05:23:46 2026 GMT
  host: www.volleythat.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Volleythat Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Volley, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Volley
provider_slug: volleythat-com
slug: volleythat-com-domain-security
source_filename: volleythat-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-29'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.volleythat.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 28 05:23:46 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: volleythat.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/volleythat-com/security/volleythat-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- VoiceAI
- Gaming
- SmartTV
- Entertainment
---
