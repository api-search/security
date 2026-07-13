---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: pe.gov.br
  spf: true
hosts:
- cert_expires: Jan  6 15:25:28 2027 GMT
  host: dados.recife.pe.gov.br
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Dados Recife Pe Gov Br Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Recife City Open Data, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Recife City Open Data
provider_slug: dados-recife-pe-gov-br
slug: dados-recife-pe-gov-br-domain-security
source_filename: dados-recife-pe-gov-br-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: dados.recife.pe.gov.br\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  6 15:25:28 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: pe.gov.br\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/dados-recife-pe-gov-br/refs/heads/main/security/dados-recife-pe-gov-br-domain-security.yml
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
