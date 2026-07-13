---
description: ''
domains:
- caa:
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "ssl.com"
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: heliumtrades.com
  spf: true
hosts:
- cert_expires: Oct  5 16:45:03 2026 GMT
  host: heliumtrades.com
  hsts: true
  hsts_max_age: 259200
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Helium Heliumtrades Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Helium, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Helium
provider_slug: helium-heliumtrades
slug: helium-heliumtrades-domain-security
source_filename: helium-heliumtrades-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: heliumtrades.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  5 16:45:03 2026 GMT\n  hsts: true\n  hsts_max_age: 259200\ndomains:\n- domain: heliumtrades.com\n  dnssec: false\n  caa:\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"ssl.com\"\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/helium-heliumtrades/refs/heads/main/security/helium-heliumtrades-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Finance
- Public APIs
---
