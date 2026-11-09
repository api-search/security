---
description: ''
domains:
- caa:
  - 0 iodef "mailto:david@deadbrands.co"
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "ssl.com"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: deadbrands.co
  spf: true
hosts:
- cert_expires: Jan 10 15:50:19 2027 GMT
  host: deadbrands.co
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Deadbrands Co Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Dead Brands, LLC, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Dead Brands, LLC
provider_slug: deadbrands-co
slug: deadbrands-co-domain-security
source_filename: deadbrands-co-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-05'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: deadbrands.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 10 15:50:19 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: deadbrands.co\n  dnssec: false\n  caa:\n  - 0 iodef \"mailto:david@deadbrands.co\"\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"ssl.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/deadbrands-co/security/deadbrands-co-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- BrandRevival
- ERPConsulting
- AI Automation
- Podcasts
- Small Business
---
