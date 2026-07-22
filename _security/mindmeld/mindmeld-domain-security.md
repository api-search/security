---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: mindmeld.com
  spf: true
hosts:
- cert_expires: Oct 28 23:59:59 2026 GMT
  host: mindmeld.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Mindmeld Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for MindMeld *, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: MindMeld *
provider_slug: mindmeld
slug: mindmeld-domain-security
source_filename: mindmeld-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: mindmeld.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 28 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: mindmeld.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mindmeld/refs/heads/main/security/mindmeld-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- AI
- Conversational AI
- Chatbots
- Natural Language Processing
- Voice Interfaces
- Machine Learning
- Open Source
- Python
---
