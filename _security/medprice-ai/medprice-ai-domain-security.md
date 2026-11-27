---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: medprice.ai
  spf: true
hosts:
- cert_expires: Dec 30 23:58:28 2026 GMT
  host: medprice.ai
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Medprice AI Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Medprice AI, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Medprice AI
provider_slug: medprice-ai
slug: medprice-ai-domain-security
source_filename: medprice-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: medprice.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 30 23:58:28 2026 GMT\n  hsts: false\ndomains:\n- domain: medprice.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/medprice-ai/security/medprice-ai-domain-security.yml
summary_line: TLSv1.3
tags:
- Medical Data
- Hospital Pricing
- AI Assistant
- MCP Server
- Charge Data
- Payer Rates
---
