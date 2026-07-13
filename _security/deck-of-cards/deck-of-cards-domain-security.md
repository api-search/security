---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: deckofcardsapi.com
  spf: false
hosts:
- cert_expires: Aug 30 21:56:34 2026 GMT
  host: deckofcardsapi.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Deck Of Cards Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Deck of Cards, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Deck of Cards
provider_slug: deck-of-cards
slug: deck-of-cards-domain-security
source_filename: deck-of-cards-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: deckofcardsapi.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 30 21:56:34 2026 GMT\n  hsts: false\ndomains:\n- domain: deckofcardsapi.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/deck-of-cards/refs/heads/main/security/deck-of-cards-domain-security.yml
summary_line: TLSv1.3
tags:
- Games And Comics
- Public APIs
---
