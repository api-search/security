---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: super73.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: shopify.dev
  spf: false
hosts:
- cert_expires: Oct 27 15:51:33 2026 GMT
  host: super73.com
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
- cert_expires: Oct 27 06:12:04 2026 GMT
  host: eu.super73.com
  hsts: true
  hsts_max_age: 7889238
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Super73 Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Super73, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Super73
provider_slug: super73
slug: super73-domain-security
source_filename: super73-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-29'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: super73.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 27 15:51:33 2026 GMT\n  hsts: true\n  hsts_max_age: 7889238\n- host: shopify.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 10 06:37:15 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\n- host: eu.super73.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 27 06:12:04 2026 GMT\n  hsts: true\n  hsts_max_age: 7889238\ndomains:\n- domain: super73.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: shopify.dev\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/super73/refs/heads/main/security/super73-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Electric Bikes
- Micromobility
- E-Commerce
- Agentic Commerce
- Consumer Hardware
- MCP
- Universal Commerce Protocol
- Shopify
- Direct to Consumer
- Internet of Things
- Transportation
---
