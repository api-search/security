---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: iffcotokio.co.in
  spf: true
hosts:
- cert_expires: Mar 27 23:59:59 2027 GMT
  host: iffcotokio.co.in
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Iffco Tokio Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for IFFCO-Tokio General Insurance, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: IFFCO-Tokio General Insurance
provider_slug: iffco-tokio
slug: iffco-tokio-domain-security
source_filename: iffco-tokio-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-28'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: iffcotokio.co.in\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Mar 27 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: iffcotokio.co.in\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/iffco-tokio/security/iffco-tokio-domain-security.yml
summary_line: TLSv1.2 · HSTS · DMARC
tags:
- Insurance
- GeneralInsurance
- India
- JointVenture
- FinancialServices
---
