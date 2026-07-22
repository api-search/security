---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: aninebing.com
  spf: true
hosts:
- cert_expires: Sep 28 17:56:32 2026 GMT
  host: aninebing.com
  hsts: true
  hsts_max_age: 7889238
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Anine Bing Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Anine Bing, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Anine Bing
provider_slug: anine-bing
slug: anine-bing-domain-security
source_filename: anine-bing-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: aninebing.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 28 17:56:32 2026 GMT\n  hsts: true\n  hsts_max_age: 7889238\ndomains:\n- domain: aninebing.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/anine-bing/refs/heads/main/security/anine-bing-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Retail
- Fashion
- Apparel
- Ecommerce
- Shopify
- Agent Commerce
- MCP
---
