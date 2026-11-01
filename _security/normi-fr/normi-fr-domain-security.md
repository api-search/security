---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: normi.fr
  spf: true
hosts:
- cert_expires: Jan  3 04:41:34 2027 GMT
  host: normi.fr
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Normi Fr Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for normi-fr, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: normi-fr
provider_slug: normi-fr
slug: normi-fr-domain-security
source_filename: normi-fr-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: normi.fr\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  3 04:41:34 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: normi.fr\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/normi-fr/security/normi-fr-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Real Estate
- Data API
- French Market
- Property Transactions
---
