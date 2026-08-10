---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: voyagefoods.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: shopify.dev
  spf: false
hosts:
- cert_expires: Sep 15 11:45:02 2026 GMT
  host: voyagefoods.com
  hsts: true
  hsts_max_age: 7889238
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 10 06:37:15 2026 GMT
  host: shopify.dev
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Voyage Foods Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Voyage Foods, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: Voyage Foods
provider_slug: voyage-foods
slug: voyage-foods-domain-security
source_filename: voyage-foods-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-05'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: voyagefoods.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 15 11:45:02 2026 GMT\n  hsts: true\n  hsts_max_age: 7889238\n- host: shopify.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 10 06:37:15 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: voyagefoods.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: shopify.dev\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/voyage-foods/refs/heads/main/security/voyage-foods-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Food and Beverage
- Consumer Packaged Goods
- Ecommerce
- Agentic Commerce
- Universal Commerce Protocol
- MCP
- GraphQL
- Shopify
- Food Technology
---
