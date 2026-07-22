---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: lordandtaylor.com
  spf: true
hosts:
- cert_expires: Aug 29 05:19:32 2026 GMT
  host: lordandtaylor.com
  hsts: true
  hsts_max_age: 7889238
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Lordandtaylor Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Lord & Taylor, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Lord & Taylor
provider_slug: lordandtaylor
slug: lordandtaylor-domain-security
source_filename: lordandtaylor-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: lordandtaylor.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 29 05:19:32 2026 GMT\n  hsts: true\n  hsts_max_age: 7889238\ndomains:\n- domain: lordandtaylor.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/lordandtaylor/refs/heads/main/security/lordandtaylor-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Retail
- E-Commerce
- Apparel
- Shopping
- Department Store
- Agentic Commerce
- MCP
---
