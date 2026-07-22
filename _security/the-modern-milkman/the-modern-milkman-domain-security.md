---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: themodernmilkman.co.uk
  spf: true
hosts:
- cert_expires: Sep 16 00:20:10 2026 GMT
  host: themodernmilkman.co.uk
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: The Modern Milkman Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for The Modern Milkman, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: The Modern Milkman
provider_slug: the-modern-milkman
slug: the-modern-milkman-domain-security
source_filename: the-modern-milkman-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: themodernmilkman.co.uk\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 16 00:20:10 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: themodernmilkman.co.uk\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/the-modern-milkman/refs/heads/main/security/the-modern-milkman-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Consumer
- Grocery Delivery
- Direct to Consumer
- Sustainability
- Subscription
- United Kingdom
- Food and Beverage
---
