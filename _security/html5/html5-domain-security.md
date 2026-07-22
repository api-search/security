---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: whatwg.org
  spf: true
hosts:
- cert_expires: Aug 23 02:20:30 2026 GMT
  host: html.spec.whatwg.org
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Html5 Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for HTML5, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: HTML5
provider_slug: html5
slug: html5-domain-security
source_filename: html5-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: html.spec.whatwg.org\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Aug 23 02:20:30 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: whatwg.org\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/html5/refs/heads/main/security/html5-domain-security.yml
summary_line: TLSv1.2 · HSTS
tags:
- Frontend
- HTML5
- Living Standard
- Markup Language
- Multimedia
- Semantic Web
- W3C
- Web Development
- WHATWG
---
