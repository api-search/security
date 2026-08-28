---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: rockthebells.com
  spf: true
hosts:
- cert_expires: Nov  1 23:08:02 2026 GMT
  host: shop.rockthebells.com
  hsts: true
  hsts_max_age: 7889238
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Rock The Bells Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Rock The Bells, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Rock The Bells
provider_slug: rock-the-bells
slug: rock-the-bells-domain-security
source_filename: rock-the-bells-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-26'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: shop.rockthebells.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  1 23:08:02 2026 GMT\n  hsts: true\n  hsts_max_age: 7889238\ndomains:\n- domain: rockthebells.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/rock-the-bells/refs/heads/main/security/rock-the-bells-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Retail
- Ecommerce
- Merchandise
- Apparel
- Agentic Commerce
- Model Context Protocol
- Universal Commerce Protocol
- GraphQL
- Media
- Music
- Hip-Hop
---
