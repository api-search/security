---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: pepper.inc
  spf: false
hosts:
- cert_expires: Aug 29 04:27:14 2026 GMT
  host: www.pepper.inc
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Pepper Content Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Pepper Content, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Pepper Content
provider_slug: pepper-content
slug: pepper-content-domain-security
source_filename: pepper-content-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.pepper.inc\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 29 04:27:14 2026 GMT\n  hsts: false\ndomains:\n- domain: pepper.inc\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/pepper-content/refs/heads/main/security/pepper-content-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- Ai Ml
- Content Marketing
- SEO
- Generative Engine Optimization
- Content Strategy
- Creative
- Marketing
---
