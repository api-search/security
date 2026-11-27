---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: clevra.ai
  spf: true
hosts:
- cert_expires: Dec 19 08:16:42 2026 GMT
  host: clevra.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Clevra Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Clevra, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Clevra
provider_slug: clevra-ai
slug: clevra-ai-domain-security
source_filename: clevra-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: clevra.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 19 08:16:42 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: clevra.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/clevra-ai/security/clevra-ai-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Field Service Management
- Contractors
- Scheduling
- Invoicing
- Payments
- CRM
- MCP
- AI Assistant
---
