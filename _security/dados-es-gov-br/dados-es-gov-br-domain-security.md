---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: es.gov.br
  spf: true
hosts:
- cert_expires: Sep 15 15:57:30 2026 GMT
  host: dados.es.gov.br
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Dados Es Gov Br Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Espirito Santo Open Data, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Espirito Santo Open Data
provider_slug: dados-es-gov-br
slug: dados-es-gov-br-domain-security
source_filename: dados-es-gov-br-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: dados.es.gov.br\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Sep 15 15:57:30 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: es.gov.br\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/dados-es-gov-br/refs/heads/main/security/dados-es-gov-br-domain-security.yml
summary_line: TLSv1.2 · HSTS
tags:
- Open Data
- CKAN
- Data Catalog
- DCAT
- Government Data
- State Government
- Brazil
---
