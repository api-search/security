---
api_specs:
- filename: terminal-shop-openapi.yml
  format: yaml
  label: Terminal Products API
  slug: products
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/terminal-shop/refs/heads/main/openapi/terminal-shop-openapi.yml
- filename: terminal-shop-openapi.yml
  format: yaml
  label: Terminal Cart API
  slug: cart
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/terminal-shop/refs/heads/main/openapi/terminal-shop-openapi.yml
- filename: terminal-shop-openapi.yml
  format: yaml
  label: Terminal Orders API
  slug: orders
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/terminal-shop/refs/heads/main/openapi/terminal-shop-openapi.yml
- filename: terminal-shop-openapi.yml
  format: yaml
  label: Terminal Subscriptions API
  slug: subscriptions
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/terminal-shop/refs/heads/main/openapi/terminal-shop-openapi.yml
- filename: terminal-shop-openapi.yml
  format: yaml
  label: Terminal Addresses & Cards API
  slug: addresses-cards
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/terminal-shop/refs/heads/main/openapi/terminal-shop-openapi.yml
- filename: terminal-shop-openapi.yml
  format: yaml
  label: Terminal Profile API
  slug: profile
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/terminal-shop/refs/heads/main/openapi/terminal-shop-openapi.yml
- filename: terminal-shop-openapi.yml
  format: yaml
  label: Terminal Tokens & Apps API
  slug: tokens
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/terminal-shop/refs/heads/main/openapi/terminal-shop-openapi.yml
description: ''
domains:
- caa:
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "ssl.com"
  - 0 issue "amazonaws.com"
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: terminal.shop
  spf: true
hosts:
- cert_expires: Nov 15 23:59:59 2026 GMT
  host: www.terminal.shop
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 11 23:59:59 2026 GMT
  host: api.terminal.shop
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 11 23:59:59 2026 GMT
  host: api.dev.terminal.shop
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Terminal Shop Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Terminal, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: Terminal
provider_slug: terminal-shop
slug: terminal-shop-domain-security
source_filename: terminal-shop-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.terminal.shop\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 15 23:59:59 2026 GMT\n  hsts: false\n- host: api.terminal.shop\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 11 23:59:59 2026 GMT\n  hsts: null\n- host: api.dev.terminal.shop\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 11 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: terminal.shop\n  dnssec: true\n  caa:\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"ssl.com\"\n  - 0 issue \"amazonaws.com\"\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/terminal-shop/refs/heads/main/security/terminal-shop-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Coffee
- E-Commerce
- Developer
- SSH
- Ordering
---
