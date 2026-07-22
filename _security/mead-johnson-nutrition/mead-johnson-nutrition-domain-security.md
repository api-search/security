---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: meadjohnson.com
  spf: false
hosts:
- cert_expires: Oct  1 21:52:19 2026 GMT
  host: www.meadjohnson.com
  hsts: true
  hsts_max_age: 15724800
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Mead Johnson Nutrition Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Mead Johnson Nutrition, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Mead Johnson Nutrition
provider_slug: mead-johnson-nutrition
slug: mead-johnson-nutrition-domain-security
source_filename: mead-johnson-nutrition-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.meadjohnson.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  1 21:52:19 2026 GMT\n  hsts: true\n  hsts_max_age: 15724800\ndomains:\n- domain: meadjohnson.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mead-johnson-nutrition/refs/heads/main/security/mead-johnson-nutrition-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Consumer Goods
- Infant Formula
- Nutrition
- Pediatric
---
