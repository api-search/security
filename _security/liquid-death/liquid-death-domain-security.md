---
api_specs:
- filename: liquid-death-storefront-openapi.yml
  format: yaml
  label: Liquid Death Storefront Read-Only JSON API
  slug: liquid-death-storefront-read-only-json-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/liquid-death/refs/heads/main/openapi/liquid-death-storefront-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: forgeglobal.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: liquiddeath.com
  spf: true
hosts:
- cert_expires: Oct 19 20:15:48 2026 GMT
  host: forgeglobal.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 25 08:06:02 2026 GMT
  host: liquiddeath.com
  hsts: true
  hsts_max_age: 7889238
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  6 15:01:35 2026 GMT
  host: liquiddeath.myshopify.com
  hsts: true
  hsts_max_age: 7889238
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Liquid Death Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Liquid Death, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Liquid Death
provider_slug: liquid-death
slug: liquid-death-domain-security
source_filename: liquid-death-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-01'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: forgeglobal.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 19 20:15:48 2026 GMT\n  hsts: null\n- host: liquiddeath.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 25 08:06:02 2026 GMT\n  hsts: true\n  hsts_max_age: 7889238\n- host: liquiddeath.myshopify.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  6 15:01:35 2026 GMT\n  hsts: true\n  hsts_max_age: 7889238\ndomains:\n- domain: forgeglobal.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: liquiddeath.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/liquid-death/refs/heads/main/security/liquid-death-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Beverages
- Consumer Packaged Goods
- Direct to Consumer
- Ecommerce
- Retail
- Agentic Commerce
- Universal Commerce Protocol
- MCP
- Shopify
---
