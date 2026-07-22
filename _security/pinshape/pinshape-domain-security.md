---
description: ''
domains:
- caa:
  - 0 issue "amazon.com"
  - 0 issue "amazonaws.com"
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  dmarc: false
  dnssec: false
  domain: pinshape.com
  spf: true
hosts:
- cert_expires: Oct  6 03:05:05 2026 GMT
  host: pinshape.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Pinshape Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Pinshape, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Pinshape
provider_slug: pinshape
slug: pinshape-domain-security
source_filename: pinshape-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: pinshape.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  6 03:05:05 2026 GMT\n  hsts: false\ndomains:\n- domain: pinshape.com\n  dnssec: false\n  caa:\n  - 0 issue \"amazon.com\"\n  - 0 issue \"amazonaws.com\"\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/pinshape/refs/heads/main/security/pinshape-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- 3D Printing
- Marketplace
- Manufacturing
- Design
- Community
- Maker
- Additive Manufacturing
---
