---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: barnandwillow.com
  spf: true
hosts:
- cert_expires: Aug 26 10:14:02 2026 GMT
  host: barnandwillow.com
  hsts: true
  hsts_max_age: 7889238
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Barn And Willow Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Barn & Willow, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Barn & Willow
provider_slug: barn-and-willow
slug: barn-and-willow-domain-security
source_filename: barn-and-willow-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: barnandwillow.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 26 10:14:02 2026 GMT\n  hsts: true\n  hsts_max_age: 7889238\ndomains:\n- domain: barnandwillow.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/barn-and-willow/refs/heads/main/security/barn-and-willow-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- E-commerce
- Retail
- Home Furnishings
- Window Treatments
- Agentic Commerce
- Shopify
- Direct to Consumer
---
