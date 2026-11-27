---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: meritvalue.com
  spf: false
hosts:
- cert_expires: Feb 11 11:56:35 2027 GMT
  host: meritvalue.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: MeritValue Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for MeritValue, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=quarantine).'
provider_name: MeritValue
provider_slug: meritvalue-com
slug: meritvalue-com-domain-security
source_filename: meritvalue-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: meritvalue.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 11 11:56:35 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: meritvalue.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/meritvalue-com/security/meritvalue-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Finance
- Valuation
- SEC
- Open Data
---
