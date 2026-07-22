---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: extensity.ai
  spf: true
hosts:
- cert_expires: Sep 25 08:28:34 2026 GMT
  host: extensity.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Extensity Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Extensity, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Extensity
provider_slug: extensity
slug: extensity-domain-security
source_filename: extensity-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: extensity.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 25 08:28:34 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: extensity.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/extensity/refs/heads/main/security/extensity-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Artificial Intelligence
- Neurosymbolic AI
- Large Language Models
- Knowledge Graphs
- Developer Tools
- Open Source
- Python
- Model Context Protocol
---
