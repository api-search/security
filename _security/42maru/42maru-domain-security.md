---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: 42maru.ai
  spf: true
hosts:
- cert_expires: Aug 22 03:02:49 2026 GMT
  host: 42maru.ai
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: 42Maru Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for 42Maru, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: 42Maru
provider_slug: 42maru
slug: 42maru-domain-security
source_filename: 42maru-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: 42maru.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 22 03:02:49 2026 GMT\n  hsts: false\ndomains:\n- domain: 42maru.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/42maru/refs/heads/main/security/42maru-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Artificial Intelligence
- Machine Learning
- Natural Language Processing
- Question Answering
- Cognitive Search
- Machine Reading Comprehension
- Chatbot
- Enterprise Search
- Deep Learning
---
