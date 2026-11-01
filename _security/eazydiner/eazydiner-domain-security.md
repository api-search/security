---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: eazydiner.com
  spf: true
hosts:
- cert_expires: Mar  4 23:59:59 2027 GMT
  host: www.eazydiner.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.2
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Eazydiner Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Eazydiner, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Eazydiner
provider_slug: eazydiner
slug: eazydiner-domain-security
source_filename: eazydiner-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-25'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.eazydiner.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Mar  4 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: eazydiner.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/eazydiner/security/eazydiner-domain-security.yml
summary_line: TLSv1.2 · HSTS · DMARC
tags:
- Company
- Restaurant
- Reservation
- Deals
- India
---
