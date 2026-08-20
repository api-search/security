---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: boostedcommerce.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: primelabs.org
  spf: true
hosts:
- cert_expires: Oct 26 02:43:24 2026 GMT
  host: boostedcommerce.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 27 10:28:01 2026 GMT
  host: primelabs.org
  hsts: true
  hsts_max_age: 7889238
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  7 14:32:32 2026 GMT
  host: www.myvitalvitamins.com
  hsts: true
  hsts_max_age: 7889238
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Boosted Commerce Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Boosted Commerce, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Boosted Commerce
provider_slug: boosted-commerce
slug: boosted-commerce-domain-security
source_filename: boosted-commerce-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-08'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: boostedcommerce.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 26 02:43:24 2026 GMT\n  hsts: false\n- host: primelabs.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 27 10:28:01 2026 GMT\n  hsts: true\n  hsts_max_age: 7889238\n- host: www.myvitalvitamins.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  7 14:32:32 2026 GMT\n  hsts: true\n  hsts_max_age: 7889238\ndomains:\n- domain: boostedcommerce.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: primelabs.org\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/boosted-commerce/refs/heads/main/security/boosted-commerce-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- E-Commerce
- Retail
- Consumer Packaged Goods
- Health and Wellness
- Supplements
- Beauty
- Agentic Commerce
- Universal Commerce Protocol
- MCP
- Shopify
- Direct to Consumer
---
