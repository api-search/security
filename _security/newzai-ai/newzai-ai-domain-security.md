---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: newzai.ai
  spf: true
hosts:
- cert_expires: Dec 27 04:43:52 2026 GMT
  host: newzai.ai
  hsts: true
  hsts_max_age: 10886400
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Newzai Ai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for newzai-ai, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: newzai-ai
provider_slug: newzai-ai
slug: newzai-ai-domain-security
source_filename: newzai-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: newzai.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 27 04:43:52 2026 GMT\n  hsts: true\n  hsts_max_age: 10886400\ndomains:\n- domain: newzai.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/newzai-ai/security/newzai-ai-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- News
- AI
- Aggregation
- Personalization
- Multilingual
---
