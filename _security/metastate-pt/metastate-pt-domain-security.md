---
description: ''
domains:
- caa:
  - 0 issue "sectigo.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: metastate.pt
  spf: true
hosts:
- cert_expires: Feb 13 19:35:16 2027 GMT
  host: metastate.pt
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Metastate Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Metastate, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Metastate
provider_slug: metastate-pt
slug: metastate-pt-domain-security
source_filename: metastate-pt-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: metastate.pt\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 13 19:35:16 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: metastate.pt\n  dnssec: false\n  caa:\n  - 0 issue \"sectigo.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/metastate-pt/security/metastate-pt-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Real Estate
- Brokerage
- Artificial Intelligence
- Portugal
- Property
---
