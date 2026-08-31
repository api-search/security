---
description: ''
domains:
- caa:
  - 0 issue "digicert.com"
  - 0 issue "startcomca.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  - 0 issue "digicert.ne.jp"
  - 0 issue "geotrust.com"
  dmarc: false
  dnssec: true
  domain: ba.gov.br
  spf: true
hosts:
- host: dados.ba.gov.br
  hsts: null
  https: true
  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: unable to get local issuer certificate (_ssl.c:1082)'
kind: domain-security
layout: security
method: probed
name: Dados Ba Gov Br Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Bahia Open Data, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS; 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC absent.'
provider_name: Bahia Open Data
provider_slug: dados-ba-gov-br
slug: dados-ba-gov-br-domain-security
source_filename: dados-ba-gov-br-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: dados.ba.gov.br\n  https: true\n  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: unable to get\n    local issuer certificate (_ssl.c:1082)'\n  hsts: null\ndomains:\n- domain: ba.gov.br\n  dnssec: true\n  caa:\n  - 0 issue \"digicert.com\"\n  - 0 issue \"startcomca.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  - 0 issue \"digicert.ne.jp\"\n  - 0 issue \"geotrust.com\"\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/dados-ba-gov-br/refs/heads/main/security/dados-ba-gov-br-domain-security.yml
summary_line: DNSSEC
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
