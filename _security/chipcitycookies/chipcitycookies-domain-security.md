---
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  - 0 issue "sectigo.com"
  - 0 issue "amazon.com"
  - 0 issue "amazontrust.com"
  - 0 issue "awstrust.com"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: chipcitycookies.com
  spf: true
hosts:
- cert_expires: Nov 26 18:11:11 2026 GMT
  host: chipcitycookies.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Chipcitycookies Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Chipcitycookies, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Chipcitycookies
provider_slug: chipcitycookies
slug: chipcitycookies-domain-security
source_filename: chipcitycookies-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-08'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: chipcitycookies.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 26 18:11:11 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: chipcitycookies.com\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  - 0 issue \"sectigo.com\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"amazontrust.com\"\n  - 0 issue \"awstrust.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/chipcitycookies/refs/heads/main/security/chipcitycookies-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Bakery
- Catering
- Cookies
- E-Commerce
---
