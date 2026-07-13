---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: alexflipnote.dev
  spf: true
hosts:
- cert_expires: Oct  2 04:59:06 2026 GMT
  host: coffee.alexflipnote.dev
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Coffee Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Coffee, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Coffee
provider_slug: coffee
slug: coffee-domain-security
source_filename: coffee-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: coffee.alexflipnote.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  2 04:59:06 2026 GMT\n  hsts: false\ndomains:\n- domain: alexflipnote.dev\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/coffee/refs/heads/main/security/coffee-domain-security.yml
summary_line: TLSv1.3
tags:
- Food And Drink
- Public APIs
---
