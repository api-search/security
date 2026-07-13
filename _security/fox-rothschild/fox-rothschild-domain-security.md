---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: foxrothschild.com
  spf: true
hosts:
- cert_expires: Sep 18 11:40:41 2026 GMT
  host: www.foxrothschild.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  2 17:55:52 2026 GMT
  host: advertisinglaw.foxrothschild.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  1 18:22:31 2026 GMT
  host: californiaemploymentlaw.foxrothschild.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Fox Rothschild Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Fox Rothschild LLP, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Fox Rothschild LLP
provider_slug: fox-rothschild
slug: fox-rothschild-domain-security
source_filename: fox-rothschild-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.foxrothschild.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 18 11:40:41 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\n- host: advertisinglaw.foxrothschild.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  2 17:55:52 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: californiaemploymentlaw.foxrothschild.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  1 18:22:31 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: foxrothschild.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/fox-rothschild/refs/heads/main/security/fox-rothschild-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Law Firm
- Legal
- Professional Services
- Blogs
- RSS
- LexBlog
- Publications
- Content
---
