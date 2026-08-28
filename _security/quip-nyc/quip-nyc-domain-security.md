---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: getquip.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: shopify.dev
  spf: false
hosts:
- cert_expires: Nov  8 07:07:01 2026 GMT
  host: www.getquip.com
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
name: Quip Nyc Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Quip NYC, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Quip NYC
provider_slug: quip-nyc
slug: quip-nyc-domain-security
source_filename: quip-nyc-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-26'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nnote: >-\n  shopify.dev appears below only because it is the humanURL of the Storefront GraphQL API\n  entry — it is the platform vendor's documentation host, not a quip-controlled domain, and\n  its posture should not be read as quip's. The quip-controlled surface is www.getquip.com /\n  getquip.com: TLS 1.3, HSTS with a ~91-day max-age, DNSSEC signed, SPF and DMARC present at\n  p=quarantine, and NO CAA record published.\nhosts:\n- host: www.getquip.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  8 07:07:01 2026 GMT\n  hsts: true\n  hsts_max_age: 7889238\n- host: shopify.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 10 06:37:15 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: getquip.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: shopify.dev\n  dnssec: false\n  caa:\
  \ []\n  spf: false\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/quip-nyc/refs/heads/main/security/quip-nyc-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Oral Care
- Consumer Health
- Personal Care
- Retail
- E-Commerce
- Direct to Consumer
- Subscription
- Agentic Commerce
- Shopify
---
