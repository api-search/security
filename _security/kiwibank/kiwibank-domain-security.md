---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: kiwibank.co.nz
  spf: true
hosts:
- cert_expires: Mar  5 23:59:59 2027 GMT
  host: www.kiwibank.co.nz
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Kiwibank Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Kiwibank, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Kiwibank
provider_slug: kiwibank
slug: kiwibank-domain-security
source_filename: kiwibank-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-26'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.kiwibank.co.nz\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar  5 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: kiwibank.co.nz\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/kiwibank/security/kiwibank-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Banking
- Finance
- NewZealand
- DigitalBanking
---
