---
description: ''
domains:
- caa:
  - 0 issue "pki.goog"
  - 0 issue "sectigo.com"
  - 0 issue "letsencrypt.org"
  dmarc: false
  dnssec: false
  domain: cosmicotter.ca
  spf: false
hosts:
- cert_expires: Jan  8 19:45:19 2027 GMT
  host: cosmicotter.ca
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Cosmicotter Ca Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for cosmicotter-ca, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: cosmicotter-ca
provider_slug: cosmicotter-ca
slug: cosmicotter-ca-domain-security
source_filename: cosmicotter-ca-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-29'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: cosmicotter.ca\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  8 19:45:19 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: cosmicotter.ca\n  dnssec: false\n  caa:\n  - 0 issue \"pki.goog\"\n  - 0 issue \"sectigo.com\"\n  - 0 issue \"letsencrypt.org\"\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/cosmicotter-ca/security/cosmicotter-ca-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- 5-MeO-DMT
- Ceremonies
- Sound Bath
- Victoria
- Canada
---
