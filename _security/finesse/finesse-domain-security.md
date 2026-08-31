---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: finesse.us
  spf: false
hosts:
- cert_expires: Oct 29 02:19:32 2026 GMT
  host: finesse.us
  hsts: true
  hsts_max_age: 7889238
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Finesse Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for FINESSE, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=none).'
provider_name: FINESSE
provider_slug: finesse
slug: finesse-domain-security
source_filename: finesse-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-12'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: finesse.us\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 29 02:19:32 2026 GMT\n  hsts: true\n  hsts_max_age: 7889238\ndomains:\n- domain: finesse.us\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/finesse/refs/heads/main/security/finesse-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Retail
- E-Commerce
- fashion
- apparel
- direct-to-consumer
- agentic-commerce
- UCP
- MCP
- agent-native
- shopify
- consumer
---
