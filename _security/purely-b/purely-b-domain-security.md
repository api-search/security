---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: purelyb.com
  spf: true
hosts:
- cert_expires: Sep 10 02:16:33 2026 GMT
  host: purelyb.com
  hsts: true
  hsts_max_age: 7889238
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Purely B Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Purely B, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Purely B
provider_slug: purely-b
slug: purely-b-domain-security
source_filename: purely-b-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: purelyb.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 10 02:16:33 2026 GMT\n  hsts: true\n  hsts_max_age: 7889238\ndomains:\n- domain: purelyb.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/purely-b/refs/heads/main/security/purely-b-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Wellness
- E-Commerce
- Supplements
- Shopify
- Agentic Commerce
- MCP
---
