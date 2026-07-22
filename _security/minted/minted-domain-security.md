---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: minted.com
  spf: true
hosts:
- cert_expires: Oct 11 06:46:29 2026 GMT
  host: minted.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Minted Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Minted, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Minted
provider_slug: minted
slug: minted-domain-security
source_filename: minted-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: minted.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 11 06:46:29 2026 GMT\n  hsts: null\ndomains:\n- domain: minted.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/minted/refs/heads/main/security/minted-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- E-Commerce
- Marketplace
- Stationery
- Design
- Consumer
- Retail
---
