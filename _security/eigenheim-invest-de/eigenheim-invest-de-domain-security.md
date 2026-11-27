---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: eigenheim-invest.de
  spf: true
hosts:
- cert_expires: Jan 11 16:27:59 2027 GMT
  host: eigenheim-invest.de
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Eigenheim Invest Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Eigenheim Invest, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Eigenheim Invest
provider_slug: eigenheim-invest-de
slug: eigenheim-invest-de-domain-security
source_filename: eigenheim-invest-de-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-06'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: eigenheim-invest.de\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 11 16:27:59 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: eigenheim-invest.de\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/eigenheim-invest-de/security/eigenheim-invest-de-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Berlin
- Investment
---
