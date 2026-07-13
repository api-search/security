---
description: ''
domains:
- caa:
  - 0 issue "certificados.serpro.gov.br"
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "sectigo.com"
  - 0 issue "amazontrust.com"
  - 0 issue "sectigo.com"
  - 0 issuewild "amazontrust.com"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: df.gov.br
  spf: true
hosts:
- host: dados.df.gov.br
  https: false
kind: domain-security
layout: security
method: probed
name: Dados Df Gov Br Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Dados abertos Distrito Federal, probed live across 1 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Dados abertos Distrito Federal
provider_slug: dados-df-gov-br
slug: dados-df-gov-br-domain-security
source_filename: dados-df-gov-br-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: dados.df.gov.br\n  https: false\ndomains:\n- domain: df.gov.br\n  dnssec: false\n  caa:\n  - 0 issue \"certificados.serpro.gov.br\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"sectigo.com\"\n  - 0 issue \"amazontrust.com\"\n  - 0 issue \"sectigo.com\"\n  - 0 issuewild \"amazontrust.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/dados-df-gov-br/refs/heads/main/security/dados-df-gov-br-domain-security.yml
summary_line: DMARC
tags:
- Open Data
- CKAN
- Data Catalog
- DCAT
- Government Data
- Open Data Portal
- Brazil
---
