---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: textual.ai
  spf: true
hosts:
- cert_expires: Dec  1 11:00:44 2026 GMT
  host: textual.ai
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Textual Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Textual.ai, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Textual.ai
provider_slug: textual
slug: textual-domain-security
source_filename: textual-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: textual.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  1 11:00:44 2026 GMT\n  hsts: false\ndomains:\n- domain: textual.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/textual/security/textual-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- Artificial Intelligence
- E-Commerce
- Generative AI
- Automation
---
