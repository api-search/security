---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: parenthoods.com
  spf: true
hosts:
- cert_expires: Oct  7 09:45:39 2026 GMT
  host: parenthoods.com
  hsts: true
  hsts_max_age: 31556926
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Parenthoods Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for parenthoods, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: parenthoods
provider_slug: parenthoods
slug: parenthoods-domain-security
source_filename: parenthoods-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: parenthoods.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  7 09:45:39 2026 GMT\n  hsts: true\n  hsts_max_age: 31556926\ndomains:\n- domain: parenthoods.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/parenthoods/refs/heads/main/security/parenthoods-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Parenting
- Social Network
- Mobile
- Consumer
- Y Combinator
- Portfolio
---
