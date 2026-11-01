---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: kalicart.com
  spf: true
hosts:
- cert_expires: Jan 19 04:16:56 2027 GMT
  host: kalicart.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Kalicart Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for kalicart-com, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: kalicart-com
provider_slug: kalicart-com
slug: kalicart-com-domain-security
source_filename: kalicart-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: kalicart.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 19 04:16:56 2027 GMT\n  hsts: false\ndomains:\n- domain: kalicart.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/kalicart-com/security/kalicart-com-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- E-commerce
- WooCommerce
- AgenticCommerce
- OpenProtocol
- AI
---
