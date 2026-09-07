---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: fourthandheart.com
  spf: true
hosts:
- cert_expires: Oct 28 23:14:01 2026 GMT
  host: fourthandheart.com
  hsts: true
  hsts_max_age: 7889238
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: 4Th Heart Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for 4th & Heart, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: 4th & Heart
provider_slug: 4th-heart
slug: 4th-heart-domain-security
source_filename: 4th-heart-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-05'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: fourthandheart.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 28 23:14:01 2026 GMT\n  hsts: true\n  hsts_max_age: 7889238\ndomains:\n- domain: fourthandheart.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/4th-heart/refs/heads/main/security/4th-heart-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Food and Beverage
- Consumer Packaged Goods
- Retail
- E-Commerce
- Agentic Commerce
- Universal Commerce Protocol
- Model Context Protocol
- Shopify
- Direct to Consumer
---
