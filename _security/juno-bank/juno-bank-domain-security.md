---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: juno.com.br
  spf: true
hosts:
- host: juno.com.br
  https: false
- host: dev.juno.com.br
  https: false
kind: domain-security
layout: security
method: probed
name: Juno Bank Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Juno, probed live across 2 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Juno
provider_slug: juno-bank
slug: juno-bank-domain-security
source_filename: juno-bank-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: juno.com.br\n  https: false\n- host: dev.juno.com.br\n  https: false\ndomains:\n- domain: juno.com.br\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/juno-bank/refs/heads/main/security/juno-bank-domain-security.yml
summary_line: no transport/DNS hardening detected
tags:
- Payments
- Billing
- Subscriptions
- PIX
- Boleto
- Boleto Pix
- Credit Cards
- Marketplace
- Payment Split
- Banking as a Service
- Digital Account
- Webhooks
- Brazil
- Fintech
- EBANX
---
