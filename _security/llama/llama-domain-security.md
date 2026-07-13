---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: llama.com
  spf: true
- caa:
  - 0 issue "digicert.com; account=271b0beda0771d006aa3a6c11b05187d456d6c239b46cb5241196095b09c92af"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: meta.com
  spf: true
hosts:
- cert_expires: Jul 19 23:59:59 2026 GMT
  host: www.llama.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jul 19 23:59:59 2026 GMT
  host: llama.developer.meta.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jul 19 23:59:59 2026 GMT
  host: api.llama.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Llama Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Llama, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Llama
provider_slug: llama
slug: llama-domain-security
source_filename: llama-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.llama.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jul 19 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: llama.developer.meta.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jul 19 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\n- host: api.llama.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jul 19 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: llama.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n- domain: meta.com\n  dnssec: false\n  caa:\n  - 0 issue \"digicert.com; account=271b0beda0771d006aa3a6c11b05187d456d6c239b46cb5241196095b09c92af\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/llama/refs/heads/main/security/llama-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- AI
- Large Language Models
- Machine Learning
- Meta
- Open Source
- LLM
- Natural Language Processing
---
