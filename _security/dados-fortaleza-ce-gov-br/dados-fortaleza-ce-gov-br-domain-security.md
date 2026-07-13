---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: true
  domain: ce.gov.br
  spf: false
hosts:
- cert_expires: Sep 15 23:59:59 2026 GMT
  host: dados.fortaleza.ce.gov.br
  hsts: true
  hsts_max_age: 16070400
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Dados Fortaleza Ce Gov Br Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Fortaleza Dados Abertos, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF absent, DMARC absent.'
provider_name: Fortaleza Dados Abertos
provider_slug: dados-fortaleza-ce-gov-br
slug: dados-fortaleza-ce-gov-br-domain-security
source_filename: dados-fortaleza-ce-gov-br-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: dados.fortaleza.ce.gov.br\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Sep 15 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 16070400\ndomains:\n- domain: ce.gov.br\n  dnssec: true\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/dados-fortaleza-ce-gov-br/refs/heads/main/security/dados-fortaleza-ce-gov-br-domain-security.yml
summary_line: TLSv1.2 · HSTS · DNSSEC
tags:
- Open Data
- CKAN
- Data Catalog
- DCAT
- Government Data
- Open Data Portal
- Brazil
---
