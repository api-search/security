---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: fig-1.co
  spf: true
hosts:
- cert_expires: Sep  3 18:27:33 2026 GMT
  host: fig-1.co
  hsts: true
  hsts_max_age: 7889238
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Fig 1 Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Fig 1, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Fig 1
provider_slug: fig-1
slug: fig-1-domain-security
source_filename: fig-1-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: fig-1.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  3 18:27:33 2026 GMT\n  hsts: true\n  hsts_max_age: 7889238\ndomains:\n- domain: fig-1.co\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/fig-1/refs/heads/main/security/fig-1-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Skincare
- Beauty
- Ecommerce
- Direct-to-Consumer
- Consumer
- Shopify
---
