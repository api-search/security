---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: crawl4ai.com
  spf: true
hosts:
- cert_expires: Sep  6 08:50:28 2026 GMT
  host: crawl4ai.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Crawl4Ai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Crawl4AI, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Crawl4AI
provider_slug: crawl4ai
slug: crawl4ai-domain-security
source_filename: crawl4ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: crawl4ai.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  6 08:50:28 2026 GMT\n  hsts: false\ndomains:\n- domain: crawl4ai.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/crawl4ai/refs/heads/main/security/crawl4ai-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- AI Automation
- Web Crawling
---
