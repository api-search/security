---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: material-exchange.com
  spf: true
hosts:
- cert_expires: Oct 14 06:42:52 2026 GMT
  host: material-exchange.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Material Exchange Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Material Exchange, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Material Exchange
provider_slug: material-exchange
slug: material-exchange-domain-security
source_filename: material-exchange-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: material-exchange.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 14 06:42:52 2026 GMT\n  hsts: false\ndomains:\n- domain: material-exchange.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/material-exchange/refs/heads/main/security/material-exchange-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Company
- Marketplace
- Sourcing
- Supply Chain
- Product Development
- Materials
- Procurement
- AI Assistant
---
