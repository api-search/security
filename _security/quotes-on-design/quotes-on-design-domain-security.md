---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: quotesondesign.com
  spf: false
hosts:
- cert_expires: Aug 24 09:47:24 2026 GMT
  host: quotesondesign.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Quotes On Design Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Quotes on Design, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Quotes on Design
provider_slug: quotes-on-design
slug: quotes-on-design-domain-security
source_filename: quotes-on-design-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: quotesondesign.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 24 09:47:24 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: quotesondesign.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/quotes-on-design/refs/heads/main/security/quotes-on-design-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Personality
- Public APIs
---
