---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: relevanceai.com
  spf: true
hosts:
- cert_expires: Sep 14 02:57:06 2026 GMT
  host: relevanceai.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Relevance Ai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Relevance AI, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Relevance AI
provider_slug: relevance-ai
slug: relevance-ai-domain-security
source_filename: relevance-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: relevanceai.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 14 02:57:06 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: relevanceai.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/relevance-ai/refs/heads/main/security/relevance-ai-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- AI Agents
- AI Automation
---
