---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: wave-ai.net
  spf: true
hosts:
- cert_expires: Sep 22 10:24:17 2026 GMT
  host: wave-ai.net
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Wave Ai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Wave AI, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Wave AI
provider_slug: wave-ai
slug: wave-ai-domain-security
source_filename: wave-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: wave-ai.net\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 22 10:24:17 2026 GMT\n  hsts: false\ndomains:\n- domain: wave-ai.net\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/wave-ai/refs/heads/main/security/wave-ai-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- Artificial Intelligence
- Music
- Generative AI
- Songwriting
- Creativity
- Machine Learning
- Consumer SaaS
---
