---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: sp.gov.br
  spf: true
hosts:
- cert_expires: Dec  9 23:59:59 2026 GMT
  host: dados.prefeitura.sp.gov.br
  hsts: false
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Dados Prefeitura Sp Gov Br Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Portal de Dados Abertos da Cidade de São Paulo, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Portal de Dados Abertos da Cidade de São Paulo
provider_slug: dados-prefeitura-sp-gov-br
slug: dados-prefeitura-sp-gov-br-domain-security
source_filename: dados-prefeitura-sp-gov-br-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: dados.prefeitura.sp.gov.br\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Dec  9 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: sp.gov.br\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/dados-prefeitura-sp-gov-br/refs/heads/main/security/dados-prefeitura-sp-gov-br-domain-security.yml
summary_line: TLSv1.2 · DMARC
tags:
- Open Data
- CKAN
- Data Catalog
- DCAT
- Government Data
- Open Data Portal
- Brazil
---
