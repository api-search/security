---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: cralo.ai
  spf: true
hosts:
- cert_expires: Jan 17 11:33:11 2027 GMT
  host: cralo.ai
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Cralo Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Cralo, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Cralo
provider_slug: cralo-ai
slug: cralo-ai-domain-security
source_filename: cralo-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: cralo.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 17 11:33:11 2027 GMT\n  hsts: false\ndomains:\n- domain: cralo.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/cralo-ai/security/cralo-ai-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- AI Agents
- Agent Tools
- Pay-per-use
- CLI
- Web Scraping
- Search
- Data Enrichment
---
