---
description: ''
domains:
- caa:
  - 0 issuewild "amazonaws.com"
  - 0 issuewild "digicert.com"
  - 0 issuewild "pki.goog"
  - 0 iodef "mailto:security@chownow.com"
  - 0 issue "amazonaws.com"
  - 0 issue "comodoca.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: chownow.com
  spf: true
hosts:
- cert_expires: Sep 12 04:58:16 2026 GMT
  host: get.chownow.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Chownow Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for ChowNow, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: ChowNow
provider_slug: chownow
slug: chownow-domain-security
source_filename: chownow-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: get.chownow.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 12 04:58:16 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: chownow.com\n  dnssec: false\n  caa:\n  - 0 issuewild \"amazonaws.com\"\n  - 0 issuewild \"digicert.com\"\n  - 0 issuewild \"pki.goog\"\n  - 0 iodef \"mailto:security@chownow.com\"\n  - 0 issue \"amazonaws.com\"\n  - 0 issue \"comodoca.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/chownow/refs/heads/main/security/chownow-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Restaurants
- Online Ordering
- Food And Beverage
- Restaurant Technology
- Point Of Sale
- Delivery
- Catering
- Marketing
- Mobile Apps
- Independent Restaurants
- Commission Free
---
