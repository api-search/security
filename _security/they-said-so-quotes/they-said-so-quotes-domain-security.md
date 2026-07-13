---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: theysaidso.com
  spf: false
hosts:
- cert_expires: Sep 12 23:27:30 2026 GMT
  host: theysaidso.com
  hsts: true
  hsts_max_age: 2592000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: They Said So Quotes Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for They Said So Quotes, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: They Said So Quotes
provider_slug: they-said-so-quotes
slug: they-said-so-quotes-domain-security
source_filename: they-said-so-quotes-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: theysaidso.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 12 23:27:30 2026 GMT\n  hsts: true\n  hsts_max_age: 2592000\ndomains:\n- domain: theysaidso.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/they-said-so-quotes/refs/heads/main/security/they-said-so-quotes-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Personality
- Public APIs
---
