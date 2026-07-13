---
description: ''
domains:
- caa:
  - 0 issue "sectigo.com"
  - 0 issue "certificados.serpro.gov.br"
  - 0 issue "letsencrypt.org"
  - 0 issue "globalsign.com"
  - 0 issue "www.digicert.com"
  dmarc: false
  dnssec: true
  domain: ro.gov.br
  spf: false
hosts:
- cert_expires: Aug 31 16:03:29 2026 GMT
  host: dados.ro.gov.br
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Dados Ro Gov Br Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Rondonia Open Data, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF absent, DMARC absent.'
provider_name: Rondonia Open Data
provider_slug: dados-ro-gov-br
slug: dados-ro-gov-br-domain-security
source_filename: dados-ro-gov-br-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: dados.ro.gov.br\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Aug 31 16:03:29 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: ro.gov.br\n  dnssec: true\n  caa:\n  - 0 issue \"sectigo.com\"\n  - 0 issue \"certificados.serpro.gov.br\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"globalsign.com\"\n  - 0 issue \"www.digicert.com\"\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/dados-ro-gov-br/refs/heads/main/security/dados-ro-gov-br-domain-security.yml
summary_line: TLSv1.2 · HSTS · DNSSEC
tags:
- Open Data
- CKAN
- Data Catalog
- DCAT
- Government Data
- Open Data Portal
- State Government
- Brazil
---
