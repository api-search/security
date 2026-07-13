---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: codepen.io
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: codepenassets.com
  spf: true
hosts:
- cert_expires: Aug 14 02:58:23 2026 GMT
  host: codepen.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 24 07:16:00 2026 GMT
  host: blog.codepen.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  5 20:29:37 2026 GMT
  host: public.codepenassets.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Codepen Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for CodePen, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: CodePen
provider_slug: codepen
slug: codepen-domain-security
source_filename: codepen-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: codepen.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 14 02:58:23 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: blog.codepen.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 24 07:16:00 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: public.codepenassets.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  5 20:29:37 2026 GMT\n  hsts: null\ndomains:\n- domain: codepen.io\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: codepenassets.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/codepen/refs/heads/main/security/codepen-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Developer Tools
- Front-End Development
- Code Playground
- Embeds
- Education
---
