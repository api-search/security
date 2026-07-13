---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: pbh.gov.br
  spf: true
hosts:
- cert_expires: Oct 17 23:59:59 2026 GMT
  host: dados.pbh.gov.br
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Dados Pbh Gov Br Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Portal de Dados Abertos – Prefeitura de Belo Horizonte, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Portal de Dados Abertos – Prefeitura de Belo Horizonte
provider_slug: dados-pbh-gov-br
slug: dados-pbh-gov-br-domain-security
source_filename: dados-pbh-gov-br-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: dados.pbh.gov.br\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 17 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: pbh.gov.br\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/dados-pbh-gov-br/refs/heads/main/security/dados-pbh-gov-br-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Open Data
- CKAN
- Data Catalog
- DCAT
- Government Data
- Open Data Portal
- Brazil
---
