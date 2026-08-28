---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: packable.com
  spf: true
hosts:
- cert_expires: Nov 24 05:06:14 2026 GMT
  host: www.packable.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Pharmapacks Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Pharmapacks, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Pharmapacks
provider_slug: pharmapacks
slug: pharmapacks-domain-security
source_filename: pharmapacks-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-26'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.packable.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 24 05:06:14 2026 GMT\n  hsts: false\ndomains:\n- domain: packable.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/pharmapacks/refs/heads/main/security/pharmapacks-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- E-Commerce
- Marketplace
- Fulfillment
- Logistics
- Retail
- Supply Chain
- Health and Beauty
- Distribution
- Defunct
---
