---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: urbanstems.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: myshopify.com
  spf: true
hosts:
- cert_expires: Nov 29 15:58:02 2026 GMT
  host: urbanstems.com
  hsts: true
  hsts_max_age: 7889238
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  6 15:01:35 2026 GMT
  host: 274513-24.myshopify.com
  hsts: true
  hsts_max_age: 7889238
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Urbanstems Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for UrbanStems, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: UrbanStems
provider_slug: urbanstems
slug: urbanstems-domain-security
source_filename: urbanstems-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-02'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: urbanstems.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 29 15:58:02 2026 GMT\n  hsts: true\n  hsts_max_age: 7889238\n- host: 274513-24.myshopify.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  6 15:01:35 2026 GMT\n  hsts: true\n  hsts_max_age: 7889238\ndomains:\n- domain: urbanstems.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: myshopify.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/urbanstems/refs/heads/main/security/urbanstems-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Commerce
- E-Commerce
- Retail
- Flowers
- Gifting
- Agentic Commerce
- Universal Commerce Protocol
- Model Context Protocol
- Shopify
- Direct to Consumer
---
