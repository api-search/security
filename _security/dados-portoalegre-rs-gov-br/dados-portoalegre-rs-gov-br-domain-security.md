---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: rs.gov.br
  spf: false
hosts:
- cert_expires: Aug  2 23:59:59 2026 GMT
  host: dados.portoalegre.rs.gov.br
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Dados Portoalegre Rs Gov Br Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Dados Abertos POA, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=none).'
provider_name: Dados Abertos POA
provider_slug: dados-portoalegre-rs-gov-br
slug: dados-portoalegre-rs-gov-br-domain-security
source_filename: dados-portoalegre-rs-gov-br-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: dados.portoalegre.rs.gov.br\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug  2 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: rs.gov.br\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/dados-portoalegre-rs-gov-br/refs/heads/main/security/dados-portoalegre-rs-gov-br-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Open Data
- CKAN
- Data Catalog
- DCAT
- Government Data
- Open Data Portal
- Brazil
---
