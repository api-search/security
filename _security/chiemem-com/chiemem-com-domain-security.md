---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: chiemem.com
  spf: true
hosts:
- cert_expires: Dec 21 14:20:28 2026 GMT
  host: chiemem.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Chiemem Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Chiemem, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Chiemem
provider_slug: chiemem-com
slug: chiemem-com-domain-security
source_filename: chiemem-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-03'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: chiemem.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 21 14:20:28 2026 GMT\n  hsts: false\ndomains:\n- domain: chiemem.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/chiemem-com/security/chiemem-com-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Marketplace
- Prompts
- Artificial Intelligence
- Generative AI
- Digital Content
- Japan
- MCP
---
