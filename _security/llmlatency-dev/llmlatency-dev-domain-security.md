---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: llmlatency.dev
  spf: true
hosts:
- cert_expires: Dec 19 13:56:40 2026 GMT
  host: llmlatency.dev
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Llmlatency Dev Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for llmlatency-dev, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: llmlatency-dev
provider_slug: llmlatency-dev
slug: llmlatency-dev-domain-security
source_filename: llmlatency-dev-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: llmlatency.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 19 13:56:40 2026 GMT\n  hsts: false\ndomains:\n- domain: llmlatency.dev\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/llmlatency-dev/security/llmlatency-dev-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Company
- AI
- Latency
- Monitoring
- Performance
---
