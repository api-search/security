---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: cocktailline.de
  spf: false
hosts:
- cert_expires: Apr 10 23:59:59 2027 GMT
  host: cocktailline.de
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Cocktailline Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Cocktailline, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=reject).'
provider_name: Cocktailline
provider_slug: cocktailline-de
slug: cocktailline-de-domain-security
source_filename: cocktailline-de-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: cocktailline.de\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Apr 10 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: cocktailline.de\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/cocktailline-de/security/cocktailline-de-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Cocktails
- Recipes
- Food and Beverage
- Ingredient Finder
- MCP
- Germany
- Consumer
---
