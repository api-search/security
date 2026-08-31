---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: true
  domain: sc.gov.br
  spf: false
hosts:
- cert_expires: Sep  1 02:07:33 2026 GMT
  host: dados.sc.gov.br
  hsts: false
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Dados Sc Gov Br Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Santa Catarina Open Data, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF absent, DMARC absent.'
provider_name: Santa Catarina Open Data
provider_slug: dados-sc-gov-br
slug: dados-sc-gov-br-domain-security
source_filename: dados-sc-gov-br-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: dados.sc.gov.br\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Sep  1 02:07:33 2026 GMT\n  hsts: false\ndomains:\n- domain: sc.gov.br\n  dnssec: true\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/dados-sc-gov-br/refs/heads/main/security/dados-sc-gov-br-domain-security.yml
summary_line: TLSv1.2 · DNSSEC
tags:
- Open Data
- CKAN
- Data Catalog
- DCAT
- Government Data
- State Government
- Brazil
---
