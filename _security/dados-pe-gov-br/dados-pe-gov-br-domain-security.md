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
- cert_expires: Sep  4 16:53:30 2026 GMT
  host: dados.pe.gov.br
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Dados Pe Gov Br Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Pernambuco Open Data, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Pernambuco Open Data
provider_slug: dados-pe-gov-br
slug: dados-pe-gov-br-domain-security
source_filename: dados-pe-gov-br-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: dados.pe.gov.br\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  4 16:53:30 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: pe.gov.br\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/dados-pe-gov-br/refs/heads/main/security/dados-pe-gov-br-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Open Data
- CKAN
- Data Catalog
- DCAT
- Government Data
- State Government
- Brazil
---
