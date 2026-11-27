---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: agenticaffiliate.ai
  spf: false
hosts:
- cert_expires: Jan  7 15:03:47 2027 GMT
  host: agenticaffiliate.ai
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Affiliate MCP Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Affiliate MCP, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=none).'
provider_name: Affiliate MCP
provider_slug: agenticaffiliate-ai
slug: agenticaffiliate-ai-domain-security
source_filename: agenticaffiliate-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-01'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: agenticaffiliate.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  7 15:03:47 2027 GMT\n  hsts: false\ndomains:\n- domain: agenticaffiliate.ai\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/agenticaffiliate-ai/security/agenticaffiliate-ai-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Affiliates
- Automation
- Artificial Intelligence
- Open Source
- Local-First
---
