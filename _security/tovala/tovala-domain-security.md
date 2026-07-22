---
description: ''
domains:
- caa:
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "ssl.com"
  - 0 issue "amazonaws.com"
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: tovala.com
  spf: true
hosts:
- cert_expires: Oct 16 14:37:35 2026 GMT
  host: www.tovala.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 15 23:59:59 2026 GMT
  host: api.tovala.com
  hsts: false
  https: true
  note: private mobile-app API host (no public developer program); root returns a friendly redirect message to tovala.com
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Tovala Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Tovala, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Tovala
provider_slug: tovala
slug: tovala-domain-security
source_filename: tovala-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.tovala.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 16 14:37:35 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.tovala.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 15 23:59:59 2026 GMT\n  hsts: false\n  note: private mobile-app API host (no public developer program); root returns\n    a friendly redirect message to tovala.com\ndomains:\n- domain: tovala.com\n  dnssec: false\n  caa:\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"ssl.com\"\n  - 0 issue \"amazonaws.com\"\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tovala/refs/heads/main/security/tovala-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Food
- Meal Delivery
- Smart Ovens
- Kitchen Appliances
- Internet of Things
- Consumer
- Food Technology
---
