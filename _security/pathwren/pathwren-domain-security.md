---
api_specs:
- filename: openapi.json
  format: json
  label: AI Crawler Index
  slug: ai-crawler-index
  spec_type: OpenAPI
  url: https://www.pathwren.workers.dev/openapi.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: workers.dev
  spf: true
hosts:
- cert_expires: Nov 29 20:21:16 2026 GMT
  host: www.pathwren.workers.dev
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Pathwren Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for AI Crawler Index, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: AI Crawler Index
provider_slug: pathwren
slug: pathwren-domain-security
source_filename: pathwren-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-01'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.pathwren.workers.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 29 20:21:16 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: workers.dev\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/pathwren/refs/heads/main/security/pathwren-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- AI crawlers
- web crawlers
- robots.txt
- user agents
- bot detection
- GPTBot
- ClaudeBot
- crawler IP ranges
- llms.txt
- open data
---
