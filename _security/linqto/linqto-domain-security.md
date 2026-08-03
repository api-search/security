---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: linqto.com
  spf: true
hosts:
- cert_expires: Sep 29 17:26:49 2026 GMT
  host: www.linqto.com
  hsts: true
  hsts_max_age: 31536000
  http_status: 200
  https: true
  server: nginx (WordPress)
  tls_version: TLSv1.3
- cert_expires: Feb  5 23:59:59 2027 GMT
  host: app.linqto.com
  hsts: true
  hsts_include_subdomains: true
  hsts_max_age: 31536000
  hsts_preload: true
  http_status: 200
  https: true
  note: single-page investor application; all unknown paths return the SPA HTML shell with 200
  server: AmazonS3
  tls_version: TLSv1.3
- cert_expires: Feb  4 23:59:59 2027 GMT
  host: api.app.linqto.com
  hsts: true
  hsts_include_subdomains: true
  hsts_max_age: 63072000
  hsts_preload: true
  http_status: 404
  https: true
  note: private session-authenticated backend for the investor app; internally routes under a /web2 prefix and returns Spring-style JSON 404 envelopes. Sends 'access-control-allow-origin +' and a restrictive frame-ancestors CSP. Not a public API.
  server: Apache
  tls_version: TLSv1.2
- cert_expires: Feb  4 23:59:59 2027 GMT
  host: blog.linqto.com
  hsts: false
  http_status: 301
  https: true
  note: redirects to https://www.linqto.com/blog/
  server: awselb/2.0
  tls_version: TLSv1.2
- host: help.linqto.com
  hsts: null
  http_status: 409
  https: false
  note: DNS resolves to HubSpot knowledge-base hosting (group38.sites.hscoscdn30.net) but the TLS certificate is not provisioned - HTTPS fails with a handshake_failure alert and HTTP returns 409. The published help center is effectively unreachable.
  tls_version: null
kind: domain-security
layout: security
method: probed
name: Linqto Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Linqto, probed live across 5 host(s) and 1 registrable domain(s). 4 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Linqto
provider_slug: linqto
slug: linqto-domain-security
source_filename: linqto-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-01'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml hosts + hosts discovered during contract discovery\nnote: developer.wordpress.org (the humanURL of the WordPress REST API entry) is a third-party\n  documentation host and is excluded; only Linqto-operated hosts are recorded here.\nhosts:\n- host: www.linqto.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 29 17:26:49 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n  http_status: 200\n  server: nginx (WordPress)\n- host: app.linqto.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  5 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n  hsts_include_subdomains: true\n  hsts_preload: true\n  http_status: 200\n  server: AmazonS3\n  note: single-page investor application; all unknown paths return the SPA HTML shell with 200\n- host: api.app.linqto.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Feb  4 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age:\
  \ 63072000\n  hsts_include_subdomains: true\n  hsts_preload: true\n  http_status: 404\n  server: Apache\n  note: private session-authenticated backend for the investor app; internally routes under\n    a /web2 prefix and returns Spring-style JSON 404 envelopes. Sends\n    'access-control-allow-origin +' and a restrictive frame-ancestors CSP. Not a public API.\n- host: blog.linqto.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Feb  4 23:59:59 2027 GMT\n  hsts: false\n  http_status: 301\n  server: awselb/2.0\n  note: redirects to https://www.linqto.com/blog/\n- host: help.linqto.com\n  https: false\n  tls_version: null\n  hsts: null\n  http_status: 409\n  note: DNS resolves to HubSpot knowledge-base hosting (group38.sites.hscoscdn30.net) but the\n    TLS certificate is not provisioned - HTTPS fails with a handshake_failure alert and HTTP\n    returns 409. The published help center is effectively unreachable.\ndomains:\n- domain: linqto.com\n  dnssec: false\n  caa: []\n  spf:\
  \ true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/linqto/refs/heads/main/security/linqto-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Private Markets
- Pre-IPO
- Secondary Market
- Investing
- Fintech
- Equity
- Accredited Investors
- Venture Capital
---
