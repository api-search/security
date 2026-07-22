---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: ecosoulhome.com
  spf: true
hosts:
- cert_expires: Aug 31 05:31:02 2026 GMT
  host: www.ecosoulhome.com
  hsts: true
  hsts_max_age: 7889238
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Ecosoul Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for EcoSoul Home, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: EcoSoul Home
provider_slug: ecosoul
slug: ecosoul-domain-security
source_filename: ecosoul-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.ecosoulhome.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 31 05:31:02 2026 GMT\n  hsts: true\n  hsts_max_age: 7889238\ndomains:\n- domain: ecosoulhome.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ecosoul/refs/heads/main/security/ecosoul-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Consumer
- Sustainability
- Home Goods
- Compostable
- Tableware
- Retail
- E-Commerce
- Shopify
- Agentic Commerce
---
