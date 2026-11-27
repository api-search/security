---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: oncarousel.com
  spf: true
hosts:
- cert_expires: Jan  8 02:51:20 2027 GMT
  host: oncarousel.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Carousel Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Carousel, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Carousel
provider_slug: oncarousel-com
slug: oncarousel-com-domain-security
source_filename: oncarousel-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: oncarousel.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  8 02:51:20 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: oncarousel.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/oncarousel-com/security/oncarousel-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Fintech
- Lending
- Tenant Screening
- API Platform
---
