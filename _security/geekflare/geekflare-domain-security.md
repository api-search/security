---
description: ''
domains:
- caa:
  - 0 issue "awstrust.com"
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "ssl.com"
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: geekflare.com
  spf: true
hosts:
- cert_expires: Aug 11 16:55:29 2026 GMT
  host: apidocs.geekflare.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Geekflare Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for GeekFlare, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: GeekFlare
provider_slug: geekflare
slug: geekflare-domain-security
source_filename: geekflare-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: apidocs.geekflare.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 11 16:55:29 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: geekflare.com\n  dnssec: true\n  caa:\n  - 0 issue \"awstrust.com\"\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"ssl.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/geekflare/refs/heads/main/security/geekflare-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Development
- Public APIs
---
