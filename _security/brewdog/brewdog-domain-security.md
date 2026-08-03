---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: brewdog.com
  spf: true
hosts:
- cert_expires: Sep 21 05:54:33 2026 GMT
  host: www.brewdog.com
  hsts: true
  hsts_max_age: 7889238
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 20 23:43:33 2026 GMT
  host: brewdog.com
  hsts: true
  hsts_max_age: 7889238
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Brewdog Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for BrewDog, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: BrewDog
provider_slug: brewdog
slug: brewdog-domain-security
source_filename: brewdog-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-02'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.brewdog.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 21 05:54:33 2026 GMT\n  hsts: true\n  hsts_max_age: 7889238\n- host: brewdog.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 20 23:43:33 2026 GMT\n  hsts: true\n  hsts_max_age: 7889238\ndomains:\n- domain: brewdog.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/brewdog/refs/heads/main/security/brewdog-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Food and Beverage
- Beer
- Brewing
- Retail
- eCommerce
- Consumer Packaged Goods
- Hospitality
- Agentic Commerce
- Shopify
---
