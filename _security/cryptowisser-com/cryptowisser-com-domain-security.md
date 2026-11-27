---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: cryptowisser.com
  spf: true
hosts:
- cert_expires: Jan 16 11:12:55 2027 GMT
  host: cryptowisser.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Cryptowisser Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Cryptowisser, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Cryptowisser
provider_slug: cryptowisser-com
slug: cryptowisser-com-domain-security
source_filename: cryptowisser-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: cryptowisser.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 16 11:12:55 2027 GMT\n  hsts: false\ndomains:\n- domain: cryptowisser.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/cryptowisser-com/security/cryptowisser-com-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- News
- Guides
- Reviews
- Exchange
- Wallets
---
