---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: kineuphorics.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: myshopify.com
  spf: true
hosts:
- cert_expires: Aug 30 11:56:01 2026 GMT
  host: www.kineuphorics.com
  hsts: true
  hsts_max_age: 7889238
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  6 15:01:35 2026 GMT
  host: kin-cocktails.myshopify.com
  hsts: true
  hsts_max_age: 7889238
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Kin Euphorics Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Kin Euphorics, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Kin Euphorics
provider_slug: kin-euphorics
slug: kin-euphorics-domain-security
source_filename: kin-euphorics-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.kineuphorics.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 30 11:56:01 2026 GMT\n  hsts: true\n  hsts_max_age: 7889238\n- host: kin-cocktails.myshopify.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  6 15:01:35 2026 GMT\n  hsts: true\n  hsts_max_age: 7889238\ndomains:\n- domain: kineuphorics.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: myshopify.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/kin-euphorics/refs/heads/main/security/kin-euphorics-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Beverages
- Non-Alcoholic
- Functional Beverage
- Adaptogens
- Nootropics
- Consumer Packaged Goods
- Ecommerce
- Shopify
- Direct to Consumer
- Agentic Commerce
- UCP
- MCP
---
