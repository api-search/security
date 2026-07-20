---
description: ''
domains:
- caa:
  - 0 issue "godaddy.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "ssl.com"
  - 0 issue "symantec.com"
  - 0 issue "amazon.com"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: honest.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: shopify.com
  spf: true
hosts:
- cert_expires: Feb  2 23:59:59 2027 GMT
  host: honest.com
  hsts: true
  hsts_max_age: 7889238
  https: true
  tls_version: TLSv1.2
- cert_expires: Sep 10 18:18:50 2026 GMT
  host: shopify.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Honest Company Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Honest Company, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.2); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Honest Company
provider_slug: honest-company
slug: honest-company-domain-security
source_filename: honest-company-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: honest.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Feb  2 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 7889238\n- host: shopify.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 10 18:18:50 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: honest.com\n  dnssec: false\n  caa:\n  - 0 issue \"godaddy.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"ssl.com\"\n  - 0 issue \"symantec.com\"\n  - 0 issue \"amazon.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: shopify.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/honest-company/refs/heads/main/security/honest-company-domain-security.yml
summary_line: TLSv1.2 · HSTS · DMARC
tags:
- Company
- Consumer Goods
- E-commerce
- Retail
- Baby Care
- Personal Care
- Beauty
- Shopify
- Agentic Commerce
- MCP
- UCP
---
