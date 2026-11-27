---
description: ''
domains:
- caa:
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "globalsign.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "sectigo.com"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: golfwithdiscs.com
  spf: true
hosts:
- cert_expires: Nov 28 10:56:26 2026 GMT
  host: golfwithdiscs.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Golf With Discs Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Golf With Discs, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Golf With Discs
provider_slug: golfwithdiscs-com
slug: golfwithdiscs-com-domain-security
source_filename: golfwithdiscs-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-10'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: golfwithdiscs.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 28 10:56:26 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: golfwithdiscs.com\n  dnssec: false\n  caa:\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"globalsign.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"sectigo.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/golfwithdiscs-com/security/golfwithdiscs-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Disc Golf
- Sports
- Community
- Reviews
- Tools
- Company
---
