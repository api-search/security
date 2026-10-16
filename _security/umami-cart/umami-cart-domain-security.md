---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: umamicart.com
  spf: false
hosts:
- cert_expires: Jan 10 11:48:48 2027 GMT
  host: umamicart.com
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Umami Cart Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Umami Cart, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Umami Cart
provider_slug: umami-cart
slug: umami-cart-domain-security
source_filename: umami-cart-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-12'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: umamicart.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 10 11:48:48 2027 GMT\n  hsts: null\ndomains:\n- domain: umamicart.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/umami-cart/refs/heads/main/security/umami-cart-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- Food
- Recipes
- AsianCuisine
- Cooking
---
