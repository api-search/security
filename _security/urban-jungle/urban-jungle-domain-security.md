---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: myurbanjungle.com
  spf: true
hosts:
- cert_expires: Dec 22 23:59:59 2026 GMT
  host: myurbanjungle.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
- cert_expires: Dec 22 23:59:59 2026 GMT
  host: api.myurbanjungle.com
  hsts: false
  https: true
  note: Answers HTTP 200 with a two-byte "OK" body and access-control-allow-origin "*". Every specification and .well-known path 404s. Added manually this round; it is not an apis.yml baseURL because no documented API is served from it.
  server: gunicorn
  tls_version: TLSv1.2
- cert_expires: Oct 23 13:51:06 2026 GMT
  host: hello.myurbanjungle.com
  hsts: false
  https: true
  note: Unbounce/Cloudflare marketing host serving the affiliate-programme landing page. HEAD / returns 404; /partner-with-us/ returns 200.
  server: cloudflare
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Urban Jungle Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Urban Jungle, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.2); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Urban Jungle
provider_slug: urban-jungle
slug: urban-jungle-domain-security
source_filename: urban-jungle-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-25'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: myurbanjungle.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Dec 22 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.myurbanjungle.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Dec 22 23:59:59 2026 GMT\n  hsts: false\n  server: gunicorn\n  note: >-\n    Answers HTTP 200 with a two-byte \"OK\" body and access-control-allow-origin\n    \"*\". Every specification and .well-known path 404s. Added manually this\n    round; it is not an apis.yml baseURL because no documented API is served\n    from it.\n- host: hello.myurbanjungle.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 23 13:51:06 2026 GMT\n  hsts: false\n  server: cloudflare\n  note: >-\n    Unbounce/Cloudflare marketing host serving the affiliate-programme landing\n    page. HEAD / returns 404; /partner-with-us/ returns 200.\ndomains:\n-\
  \ domain: myurbanjungle.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/urban-jungle/refs/heads/main/security/urban-jungle-domain-security.yml
summary_line: TLSv1.2 · HSTS · DMARC
tags:
- Insurance
- United Kingdom
- Insurtech
- Property and Casualty
- Home Insurance
- Renters Insurance
- Embedded Insurance
- Underwriting
- Brokers
- Direct to Consumer
---
