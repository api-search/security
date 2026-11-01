---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: humantalk.io
  spf: true
hosts:
- cert_expires: Dec 15 06:11:57 2026 GMT
  host: humantalk.io
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Humantalk Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for HumanPal.io, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: HumanPal.io
provider_slug: humantalk
slug: humantalk-domain-security
source_filename: humantalk-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: humantalk.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 15 06:11:57 2026 GMT\n  hsts: false\ndomains:\n- domain: humantalk.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/humantalk/security/humantalk-domain-security.yml
summary_line: TLSv1.3
tags:
- AI
- Content Generation
- Text-to-Speech
- Marketing
- SaaS
---
