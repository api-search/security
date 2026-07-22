---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: true
  domain: chordcommerce.com
  spf: false
hosts:
- cert_expires: Sep 27 06:16:54 2026 GMT
  host: www.chordcommerce.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Chord Commerce Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Chord, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF absent, DMARC absent.'
provider_name: Chord
provider_slug: chord-commerce
slug: chord-commerce-domain-security
source_filename: chord-commerce-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.chordcommerce.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 27 06:16:54 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: chordcommerce.com\n  dnssec: true\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/chord-commerce/refs/heads/main/security/chord-commerce-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC
tags:
- Commerce
- Composable Commerce
- Headless Commerce
- Order Management
- OMS
- Customer Data Platform
- CDP
- Event Tracking
- Commerce Analytics
- Customer Lifetime Value
- AI Agents
- Commerce Copilot
- Solidus
- Spree
- Ruby On Rails
- Shopify
- DTC
- Direct To Consumer
---
