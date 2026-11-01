---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: agentpay.shop
  spf: true
hosts:
- cert_expires: Jan 16 16:11:09 2027 GMT
  host: agentpay.shop
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Agentpay Shop Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for agentpay-shop, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: agentpay-shop
provider_slug: agentpay-shop
slug: agentpay-shop-domain-security
source_filename: agentpay-shop-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: agentpay.shop\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 16 16:11:09 2027 GMT\n  hsts: null\ndomains:\n- domain: agentpay.shop\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/agentpay-shop/security/agentpay-shop-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Payments
- Crypto
- AI
- Non-custodial
- AgentPay
---
