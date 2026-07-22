---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: boletosqubit.co
  spf: false
hosts:
- cert_expires: Sep  1 22:43:05 2026 GMT
  host: boletosqubit.co
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Qubit Smart Tickets Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Qubit Smart Tickets, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=none).'
provider_name: Qubit Smart Tickets
provider_slug: qubit-smart-tickets
slug: qubit-smart-tickets-domain-security
source_filename: qubit-smart-tickets-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: boletosqubit.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  1 22:43:05 2026 GMT\n  hsts: false\ndomains:\n- domain: boletosqubit.co\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/qubit-smart-tickets/refs/heads/main/security/qubit-smart-tickets-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Ticketing
- Events
- Entertainment
- Payments
- Colombia
- Latin America
---
