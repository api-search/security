---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: intellics.ai
  spf: false
hosts:
- cert_expires: Feb  2 07:58:59 2027 GMT
  host: intellics.ai
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Intellics K.K. Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Intellics K.K., probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF absent, DMARC present (p=none).'
provider_name: Intellics K.K.
provider_slug: intellics-ai
slug: intellics-ai-domain-security
source_filename: intellics-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-12'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: intellics.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  2 07:58:59 2027 GMT\n  hsts: false\ndomains:\n- domain: intellics.ai\n  dnssec: true\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/intellics-ai/security/intellics-ai-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Artificial Intelligence
- Security
- Performance
- Consulting
- Japan
---
