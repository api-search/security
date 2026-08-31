---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: chordcommerce.com
  spf: false
- caa:
  - 0 issue "ssl.com"
  - 0 issuewild "amazon.com"
  - 0 issuewild "comodoca.com"
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: chord.co
  spf: true
hosts:
- cert_expires: Sep 27 06:16:54 2026 GMT
  host: www.chordcommerce.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 20 12:01:56 2026 GMT
  host: docs.chord.co
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 26 11:09:16 2026 GMT
  host: mcp.chord.co
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Chord Commerce Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Chord, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF absent, DMARC present (p=none).'
provider_name: Chord
provider_slug: chord-commerce
slug: chord-commerce-domain-security
source_filename: chord-commerce-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.chordcommerce.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 27 06:16:54 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: docs.chord.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 20 12:01:56 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: mcp.chord.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 26 11:09:16 2026 GMT\n  hsts: null\ndomains:\n- domain: chordcommerce.com\n  dnssec: true\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: none\n- domain: chord.co\n  dnssec: false\n  caa:\n  - 0 issue \"ssl.com\"\n  - 0 issuewild \"amazon.com\"\n  - 0 issuewild \"comodoca.com\"\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/chord-commerce/refs/heads/main/security/chord-commerce-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
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
- Direct to Consumer
---
