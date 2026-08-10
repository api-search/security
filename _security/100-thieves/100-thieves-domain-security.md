---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: 100thieves.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: shopify.dev
  spf: false
hosts:
- cert_expires: Oct 26 17:55:02 2026 GMT
  host: 100thieves.com
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
name: 100 Thieves Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for 100 Thieves, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: 100 Thieves
provider_slug: 100-thieves
slug: 100-thieves-domain-security
source_filename: 100-thieves-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-05'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: 100thieves.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 26 17:55:02 2026 GMT\n  hsts: true\n  hsts_max_age: 7889238\n- host: shopify.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 10 06:37:15 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: 100thieves.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: shopify.dev\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/100-thieves/refs/heads/main/security/100-thieves-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Esports
- Gaming
- Apparel
- Retail
- E-Commerce
- Entertainment
- Media
- Direct To Consumer
- Agentic Commerce
---
