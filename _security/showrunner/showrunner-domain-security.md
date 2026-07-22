---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: showrunner.xyz
  spf: false
hosts:
- cert_expires: Sep 21 18:10:43 2026 GMT
  host: showrunner.xyz
  hsts: true
  hsts_max_age: 31556952
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Showrunner Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Showrunner, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Showrunner
provider_slug: showrunner
slug: showrunner-domain-security
source_filename: showrunner-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: showrunner.xyz\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 21 18:10:43 2026 GMT\n  hsts: true\n  hsts_max_age: 31556952\ndomains:\n- domain: showrunner.xyz\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/showrunner/refs/heads/main/security/showrunner-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Ai
- Generative AI
- Animation
- Entertainment
- Media
- Streaming
---
